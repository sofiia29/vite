<script setup>
import {RouterLink, RouterView} from 'vue-router'
import OrangeBtn from '@/components/orange_btn.vue'
import HeaderSite from '@/components/header.vue'
import Txt1 from '@/components/text_block1.vue'
</script>

<template>
  <div>
    <!-- <OrangeBtn/> -->
    <HeaderSite/>
    <Txt1/>

  </div>


</template>

<style>
body {
  font-family: 'Montserrat Alternates';
  margin: 0;
  overflow-x: hidden;
}

.container {
  width: 1532px;
  margin: auto;
}
</style>
