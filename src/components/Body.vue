<template>
    <div>
      <div class="row">
         <div class="col-sm-12" style="margin: 30px">
             <img src="../assets/1654675936.jpg" alt="">
         </div>
      </div>

      <TopProducts :products="topProductList"></TopProducts>
    
       <VueprojectFilter></VueprojectFilter>
       <MainProductsVue :products="products"></MainProductsVue>
      

    </div>
</template>

<script>
import TopProducts from '../components/TopProducts.vue'
import MainProductsVue from '../components/MainProducts.vue'

import VueprojectFilter from '../components/Filter.vue'
export default {
    name: 'BodyVue',
      components: {
  
    TopProducts,
    MainProductsVue,
    
    VueprojectFilter,
   
},
    data() {
        return {
            
        };
    },
    props:{
      products:Array,
      topProductList:Array
    },
 

    methods: {
        
    },
};
</script>

<style scoped>

</style>