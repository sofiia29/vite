<template>
    <div class="counter">
        <div class="minus" @click="minus()">-</div>
        <p>{{clicks}} kg</p>
        <div class="plus" @click="plus()">+</div>
        <input type="text" v-model="clicks">
    </div>
</template>

<script>
export default {
    name: "quantity",
    data(){
        return{
            clicks: 0,
        }
    },
    methods:{
        minus(){
            if (this.clicks > 0 ){
                this.clicks -= 1
            }
        },

        plus(){
            this.clicks += 1
        },
    },
}
</script>

<style scoped>
    .counter{
      display: flex;
    }
    .minus, .plus{
        width: 28px;
        height: 32px;
        background: #8BD32E;
        color: white;
        margin: 0;
    }

    .minus{
        border-radius: 47px 0px 0px 47px;
    }

    .plus{
        border-radius: 0px 47px 47px 0px;
    }

    p{
        width: 54px;
        height: 32px;
        background: #F5F5F5;
        font-weight: 400;
        font-size: 14px;
        line-height: 24px;
        color: #666666;
        margin: 0;
    }
</style>