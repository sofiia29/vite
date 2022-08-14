<template>
  <div class="container">
    <div class="block">
      <div class="align_txt">
        <img src="./../assets/images/Ellipse 4.svg" id="pos1">
        <img src="./../assets/images/Ellipse 5.svg" id="pos2">
        <h3>Order <span id="green">fresh</span> grocery for your business</h3>
        <p>Hi! Welcome at GoodLife website! We are fruit and vegetables delivery service.
          Our goal is to make people healthier by providing them an opportunity to eat fresh and healthy food every
          day!</p>
        <OrangeBtn color="orange" value="Order now"></OrangeBtn>
      </div>
      <img src="./../assets/images/image 58.png" id="img">
    </div>
  </div>
</template>

<script>
import OrangeBtn from '@/components/orange_btn.vue'

export default {
  name: "text_block1",
  components: {
    OrangeBtn,
  },
}
</script>

<style scoped>

.block {
  display: flex;
  flex-direction: row;
  justify-content: space-between;

}

#pos1 {
  position: absolute;
  left: -40px;
  top: -27px;
  z-index: -1;
}

#pos2 {
  position: absolute;
    left: -34px;
  top: -16px;
  z-index: -1;
}

h3 {
  font-weight: 700;
  font-size: 64px;
  line-height: 80px;
  margin: 0;
}

p{
    line-height: 28px;
    font-weight: 400;
    font-size: 18px;
}

#green {
  margin: 0;
  color: #8BD32E;
}

.align_txt {
  width: 685px;
  margin-top: 183px;
  position: relative;

}

#img {
  width: 650px;
  margin-right: -111px;
  margin-top: 100px;
  object-fit: contain;
}
</style>