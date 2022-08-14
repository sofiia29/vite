<template>
   <div class="card">
           <div class="space_betw">
               <div class="sale" v-if="product.is_sale">Sale</div>
               <div class="mark">
                   <img src="./../assets/images/Star 1.svg">
                   <p>{{product.rating}}</p>
               </div>
           </div>
            <img :src="product.img">
           <div class="txt">
               <p>{{product.category}}</p>
               <h5>{{product.name}}</h5>
               <div class="price">
                   <p class="crossed">{{product.price}} $</p>
                   <p class="green">{{product.price_ifsale}} $</p>
               </div>
           </div>
           <Orange_btn value="Add to cart" color="orange" id="btn"/>
    </div> 
</template>

<script>
import Orange_btn from './orange_btn.vue';
export default {
    name: "food_card",
    props: {
        product: Object,
    },
    components: { 
        Orange_btn, 
    }
}
</script>

<style scoped>
    .card{
        padding: 24px;
        width: 323px;
        box-shadow: 0px 2px 20px rgba(116, 141, 84, 0.2);
        border-radius: 10px;
    }
    .space_betw{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .sale{
        background-color:#8BD32E;
        color: white;
        padding: 4px 16px;
        border-radius: 37px;
        font-size: 14px;
    }

    .mark{
        border: 1px solid #D9D9D9;
        border-radius: 37px;
        color: #B6B6B6;
        font-size: 14px;
    }
    .mark p{
        margin: 0;
        padding: 4px 10px;
    }

    .txt{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-bottom: 32px;
    }

    .txt p{
        margin: 0;
        color: #B6B6B6;
        font-size: 16px;
    }

    .txt h5{
        margin: 0;
        margin-top: 6px;
        margin-bottom: 10px;
        color: #1F201F;
        font-size: 18px;
        font-weight: 700px;
    }

    .price{
        display: flex;
        flex-direction: row;
        gap: 10px;
    }

    .crossed{
        text-decoration: line-through;
    }

    .green{
        color: #8BD32E;
    }

    /* #btn{
        background-color: #FDA624;
        width: 100%;
        padding: 12px 24px;
        border: none;
        border-radius: 47px;
        font-size: 16px;
        color: white;
    } */
</style>