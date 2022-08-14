<template>
  <div class="container">
    <div class="align_header">
      <img src="./../assets/images/Logo.svg">
      <div class="header_txt">
        <p>About</p>
        <p>Categories</p>
        <p>Delivery and payment</p>
        <p>Contacts</p>
        <div class="cart_backgr">
           <img src="./../assets/images/cart.svg">
            <div class="goods">1</div>
        </div>
        <OrangeBtn color="orange" value="Sign in"></OrangeBtn>
        
        
      </div>

    </div>
  </div>

</template>

<script>
import OrangeBtn from '@/components/orange_btn.vue'

export default {
  name: 'header',
  components: {
    OrangeBtn,
  },

}
</script>

<style scoped>

.align_header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin-top: 60px;
}

.header_txt {
  display: flex;
  flex-direction: row;
  gap: 37px;
  align-items: center;
}

.cart_backgr{
    position: relative;
    background: #F5F5F5;
    border-radius: 54px;
    width: 60px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.goods{
    position: absolute;
    right: 0;
    bottom: 0;
    background: #8BD32E;
    border-radius: 28px;
    color: white;
    width: 22px;
    height: 22px;
    font-weight: 700;
    font-size: 12px;
    line-height: 24px;
    text-align: center;
}
</style>