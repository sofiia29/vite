<template>
    <div class="align_header">
        <img src="./../assets/images/Logo.svg">
        <div class="header_txt">
            <p>About</p>
            <p>Categories</p>
            <p>Delivery and payment</p>
            <p>Contacts</p> 
            <img src="./../assets/images/Cart with indicator.svg">
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'header',

}
</script>

<style scoped>

    .align_header{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    .header_txt{
        display: flex;
        flex-direction: row;
        gap: 37px;
    }
</style>