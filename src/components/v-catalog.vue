<template>

<div class="top-cards">
    <v-catalog-item
    v-for="post in posts"
    :key="post.id"
    :post_data="post"

    />

</div>

</template>

<script>
import vCatalogItem from './v-catalog-item.vue'

export default{
    name: "v-catalog",
    components:{
    vCatalogItem,
},
props:{
    type: Object,
    default(){
        return{}
    }
},

    data(){
        return{
posts:[
    {id:1,
     image: "unsplash_pbrQvuKJQf8.jpg",
     name: "Кадастровые работы в отношении земельных участков"},
     {id:2,
     image: "top2.jpg",
     name: "Кадастровые работы в отношении земельных участков"},
     {id:3,
     image: "top3.jpg",
     name: "Кадастровые работы в отношении земельных участков"},
     {id:4,
     image: "top4.jpg",
     name: "Кадастровые работы в отношении земельных участков"},
     {id:5,
     image: "top5.jpg",
     name: "Кадастровые работы в отношении земельных участков"},
     {id:6,
     image: "top6.jpg",
     name: "Кадастровые работы в отношении земельных участков"},

]
        }
    }

}
</script>


<style scoped>
    .top-cards{
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 24px;
        max-width: 1280px;
        
    margin: 0 auto;
    
        
    }
    
</style>