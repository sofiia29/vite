<template>
    <div class="backgr">
        <div class="container">
            <TitleLine text='Explore categories'/>
            <div class="space_betw">
                <CategoryCard v-bind:key="item.text" :category="item" v-for="item in categories"/>
            </div>
            <CardLink text="See all"/>
            
        </div>
    </div>
    
</template>

<script>
import CategoryCard from '@/components/category_card.vue'
import TitleLine from '@/components/title.vue'
import CardLink from '@/components/link.vue'
export default {
    name:'categories_list',
    components:{
        CategoryCard,
        TitleLine,
        CardLink,
    },
    data(){
        return{
            categories:[{
                    img: "src/assets/images/all.png",
                    text: "All"
                },
                {
                    img: "src/assets/images/vegetables.png",
                    text: "Vegetables"
                },
                {
                    img: "src/assets/images/fruits.png",
                    text: "Fruits"
                },
                {
                    img: "src/assets/images/berries.png",
                    text: "Berries"
                },
                {
                    img: "src/assets/images/greens.png",
                    text: "Greens"
                },
                // {
                //     img: "src/assets/images/exotic.png",
                //     text: "Exotic"
                // }
            ]
        }
    },

}
</script>

<style scoped>

    /* body{
        font-family: 'Montserrat Alternates';
    } */

    .backgr{
        background-color: #FAFAFA;
        padding-top: 120px;
        padding-bottom: 183px;
    }

    .space_betw{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin-top: 40px;
        gap: 16px;
    }
    
</style>