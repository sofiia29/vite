<template>
    <div class="block">
        <div class="align_txt">
            <img src="./../assets/images/Ellipse 4.svg" id="pos1">
            <img src="./../assets/images/Ellipse 5.svg" id="pos2">
            <h3>Order <p id="green">fresh</p> grocery for your business</h3>
            <p>Hi! Welcome at GoodLife website! We are fruit and vegetables delivery service. 
                Our goal is to make people healthier by providing them an opportunity to eat fresh and healthy food every day!</p>
        </div>
        <img src="./../assets/images/image 58.png" id="img">
    </div>
    
</template>

<script>
export default {
    name: "text_block1",
}
</script>

<style scoped>

    .block{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    #pos1{
        position: absolute;
        left: 141.3px;
        top: 379.47px;
    }

    #pos2{
        position: absolute;
        left: 139.69px;
        top: 357.95px;
    }

    h3{
        font-weight: 700;
        font-size: 64px;
        line-height: 80px;
        margin: 0;
        display: flex;
        flex-direction: row;
    }

    #green{
        margin: 0;
        color: #8BD32E;
    }

    .align_txt{
        width: 685px;
        margin-top: 211.38px;
        margin-left: 194px;

    }

    #img{
        width: 922px;
        height: 859px;
    }
</style>