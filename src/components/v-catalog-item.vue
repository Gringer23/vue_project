<template>
    <div class="top-card">
        <div class="top-card-pic">
          <img :src=" require('../assets/images/' + post_data.image)" alt="" class="top-card-thumb">
        </div>

    <p class="top-card-desk">{{post_data.name}}</p>
    </div>
</template>

<script>


export default{
    name:"v-catalog-item",
    props:{
post_data:{
    type: Object,
    default(){
        return{}
    }
}
    },
    data(){
        return{

        }
    }
}
</script>


<style scoped>
    .top-card{
        background-color: #fff;
            box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.09);
            border-radius: 20px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 24px;
        width: 411px;
        height: 383px;
        
        }
    .top-card-desk{
        font-family: sans-serif;
        font-size: 20px;
        font-weight: 600;
        line-height: 130%;
    
    }
    .top-card-desk:hover, .top-card-desk:focus, .top-card-desk:active{
        color: #00A76B;
    }
    .top-card-pic{
        position: relative;
        width: 363px;
        height: 267px;
        
    
    } 
</style>