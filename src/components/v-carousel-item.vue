<template>
 
        <img :src=" require('../assets/images/'+ item_data.img)" alt="">
               
</template>
    
    <script>
    
    
    export default{
    name:"v-carousel-item",
    props:{
    item_data:{
        type: Object,
        default: ()=>{}
        
    }
    },
    data(){
        return{
    
        }
    }
    
    
    }
    </script>
    
    <style scoped> 
       
       
        img{
            width: 100%;
            height: 100%;
        }
      
    </style>