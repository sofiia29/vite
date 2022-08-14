<template>
  <div class="card">
            <img :src="category.img">
            <p>{{category.text}}</p>
            <OrangeBtn color="border" value="Shop now" :isRight="true"/>
        </div>
</template>

<script>

import OrangeBtn from './orange_btn.vue'

export default {
    name: "category_card",
    components:{
        OrangeBtn,
    },
    props: {
        category:Object,

    },
}
</script>

<style scoped>
    img{
        width: 150px;
        height: 150px;
    }
    .card{
        padding: 24px;
        box-shadow: 0px 2px 20px rgba(116, 141, 84, 0.2);
        border-radius: 10px;
        display: flex;
        align-items: center;
        flex-direction: column;
        width: 100%;
        background: white;
    }

    p{
        font-weight: 700;
        font-size: 16px;
        line-height: 24px;
        color: #1F201F;
    }
</style>