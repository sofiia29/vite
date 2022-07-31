<template>
    <div>
        <button :class='[{"icon-left":isLeft, "icon-right":isRight, "orange":type==="filled", "border":type==="outlined"}, color]'>
        <div v-if="isLeft" class="img"></div>Text<div v-if="isRight"></div>
        </button>
    </div>
</template>

<script>
export default {
    name: 'orange_btn',
    props: {
        isLeft: {
            type: Boolean,
            default: false,
        },
        
        isRight: {
            type: Boolean,
            default: false,

        },
        color: String,
        type: String,


    },

}
</script>

<style scoped>


    button{
        display: flex;
        align-items: center;
        font-weight: bold;
        padding: 12px 24px;
        border: none;
        border-radius: 47px;
        color: white; 
        text-align: center;       
        font-family: 'Montserrat Alternates';
    }

    .img{
        -webkit-mask-image: url(./../assets/images/vector.svg);
        -webkit-mask-repeat: no-repeat;
        background: black;
        height: 24px;
        width: 24px;
    }

    .orange{
        background: #FDA624;
    }

    .orange:hover{
        background: #FFC164;
    }

    .border{
        color: #FDA624;
        border: 1px solid #FDA624;
        background: white;    

    }
</style>