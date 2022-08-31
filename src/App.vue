<template>

    <VHeader/>
    <main class="main">
        <section class="slider">
         
<VCarousel
:carousel_data="sliderItems"
:interval="4000"
/>      

      </section>
 
  
  <section class="top">
      <div class="wrapper-full">
          <h2 class="top-title section-title">Наши услуги</h2>
      </div>

      <VCatalog
      />
 
  <input type="button" value="Все услуги" class="top-button">
  
  </section>
  </main>
<VFooter/>


</template>

<script>
import VHeader from './components/header.vue';
import vCatalogVue from './components/v-catalog.vue';
import VCatalog from './components/v-catalog.vue';
import VCarousel from './components/v-carousel.vue';
import VFooter from './components/footer.vue'

export default{
    name: "vCatalog-main",
    components:{
    vCatalogVue,
    VCatalog,
    VCarousel,
    VHeader,
    VFooter


},

data(){
    return{
       sliderItems:[
        {id: 1, name:"img1", img:"12.jpg" },
        {id: 2, name:"img2", img:"12.jpg" },
        {id: 3, name:"img3", img:"12.jpg" },
        {id: 4, name:"img4", img:"12.jpg" },
       ]

      
        
    }
}
}
</script>

<style>
    html{
        box-sizing: border-box;
    }
    * , *::before,  *::after{
    box-sizing: inherit;
    }
    body{
        font-family: 'Open Sans';
        font-style: normal;
        font-size: 16px;
        line-height: 1.2;
        font-weight: normal;
        color: #000;
        display:flex;
        flex-wrap: wrap;
        max-width: 1440px;
    }


    .main{
        width: 100%;
        
    }
    

    .top{
        margin-bottom: 113px;
    }
    
    
    .top-title{
        margin-bottom: 32px;
        margin-top: 48px;
    }
    
    
    
    .top-button{
        display: flex;
        flex-direction: row;
    align-items: center;
    justify-content: center;
    background-color: #fff;
        font-size: 16px;
        font-weight: 400;
        border-radius: 30px;
        border: 1.5px solid #00BB78;
        cursor: pointer;
        padding: 12px 28px;
        color: #00BB78;
        line-height: 22px;
        margin: 32px auto;
    }
    
    .top-button:hover{
        background-color: #00BB78;
        color: #fff;
    }
</style>
