<script setup>
import {RouterLink, RouterView} from 'vue-router'
import OrangeBtn from '@/components/orange_btn.vue'
import HeaderSite from '@/components/header.vue'
import Txt1 from '@/components/text_block1.vue'
import TitleLine from '@/components/title.vue'
import CategoriesList from './components/categories_list.vue'
import Food_card from './components/food_card.vue'
import Quantity from './components/quantity.vue'
import Food_list from './components/food_list.vue'
</script>

<template>
  <div>
    <!-- <OrangeBtn/> -->
    <HeaderSite/>
    <Txt1/>
    <CategoriesList/>
    <Food_list/>
    <Quantity/>
  </div>


</template>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@100;200;300;400;500;600;700;800&family=Roboto+Flex:opsz,wght@8..144,100;8..144,200;8..144,300;8..144,400;8..144,500;8..144,600;8..144,700;8..144,800;8..144,900;8..144,1000&display=swap');

body {
  font-family: 'Montserrat Alternates';
  margin: 0;
  overflow-x: hidden;
}

.container {
  width: 1200px;
  margin: auto;
}
</style>
