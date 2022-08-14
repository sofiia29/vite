<template>
    <div class="container">
        <TitleLine text="Featured products"/>
        <div class="space_betw">
            <Food_card v-for="item in products" :product="item" :key="item.name"/>
        </div>
        
    </div>
</template>

<script>
import Food_card from './food_card.vue';
import TitleLine from './title.vue';
export default {
    name: "food_list",
    components: { 
        Food_card,
        TitleLine,
    },
    data(){
        return{
            products: [
                {
                    is_sale: true,
                    rating: 4.7,
                    category: 'Vegetable',
                    name: 'Broccoli',
                    price: 10,
                    price_ifsale: 5,
                    img: '/src/assets/images/broccoli.png'
                },

                {
                    is_sale: true,
                    rating: 4.4,
                    category: 'Berry',
                    name: 'Cherry',
                    price: 20,
                    price_ifsale: 15,
                    img: '/src/assets/images/cherry.png'
                },

                {
                    is_sale: true,
                    rating: 5.0,
                    category: 'Fruit',
                    name: 'Apple',
                    price: 9,
                    price_ifsale: 8,
                    img: '/src/assets/images/apple.png' 
                },

                {
                    is_sale: true,
                    rating: 4.2,
                    category: 'Vegetable',
                    name: 'Tomato',
                    price: 12,
                    price_ifsale: 10,
                    img: '/src/assets/images/tomato.png'
                }
            ],

        }
    }
}
</script>

<style scoped>
    .space_betw{
        display: flex;
        flex-direction: row;
        /* justify-content: space-between; */
        margin-top: 40px;
        gap: 16px;
    }
</style>