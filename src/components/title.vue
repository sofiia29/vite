<template>
    <div class="container">
        <h2>{{text}}</h2>
        <div class="line"></div>    
    </div>
</template>

<script>
export default {
    name: "title",
    props: {
        text: String,
    }
}
</script>

<style scoped>
    h2{
        font-weight: 700;
        font-size: 36px;
        line-height: 44px;
        color: #1F201F;
        margin: 0;
        margin-bottom: 16px;
    }

    .line{
        background: #8BD32E;
        border-radius: 24px;
        width: 40px;
        height: 10px;
    }
</style>