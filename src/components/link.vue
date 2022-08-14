<template>
    <div class="link">
        <p>{{text}}</p>
        <div class="img"></div>
    </div>
</template>

<script>
export default {
    name: "link",
    props:{
        text:String,
    }
}
</script>

<style scoped>
    .link{
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        margin-top: 34px;
    }

    p{
        font-weight: 700;
        font-size: 16px;
        line-height: 24px;
        color: #8BD32E;
        margin: 0;
    }

    .img {
        -webkit-mask-image: url(./../assets/images/green_up.svg);
        -webkit-mask-repeat: no-repeat;
        background: #8BD32E;
        height: 24px;
        width: 24px;
    }

    .link:hover p{
        color: #BAEF76;
    }

    .link:hover .img{
        background: #BAEF76;
    }

</style>