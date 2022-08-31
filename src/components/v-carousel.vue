<template>

    <div class="flex-wrapper">
        <div class="slider-wrapper" :style=" {'margin-left': '-' + (110*currentSlideIndex)+ '%'}">
<VCarouselItem
v-for="item in carousel_data"
:key="item.id"
:item_data="item"
/>

        </div>


    </div>
    
</template>

<script>


import VCarouselItem from './v-carousel-item.vue';

export default{
name:"v-carousel",
components:{
    VCarouselItem,

},
props:{
carousel_data:{
    type: Array,
    default: ()=>[]
    
},
interval:{
    type: Number,
    default: 0
}

},
data(){
    return{
       currentSlideIndex: 0
       
    }

},
methods:{
nextSlide(){ 
    if(this.currentSlideIndex >= this.carousel_data.length - 1){
        this.currentSlideIndex = 0
    }else{
    this.currentSlideIndex++
}}
},
mounted(){
if(this.interval > 0){
    let vm = this; 
    setInterval(function(){
vm.nextSlide()
    }, vm.interval)

    
}
}

}
</script>

<style scoped> 
    .flex-wrapper {
        height: 672px;
        margin-top: 60px;
        width: 100%;
        overflow: hidden;
    
        
    }
    .slider-wrapper{
      
        height: 672px;
        display: flex;
        transition: all ease .5s;
        
    }
    .dots-wrapper {
    
        display: flex;
        justify-content: center;
        margin-top: 15px ;
        position: static;
    
    }
    
    .dot.active{
    
        background-color: #000;
    }
    
   
    
</style>