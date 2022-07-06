<template>
  <div class="container">
     <div class="row">
        <img style="margin:auto; margin-top:20px ;" src="../assets/ellips.jpg" alt="">
      <div class="display">
            <!-- <div class="card" style="width: 18rem;">
                <img class="card-img-top" src="../assets/1648631992.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div>

               <div class="card" style="width: 18rem;">
                <img class="card-img-top" src="../assets/1648631992.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div>

               <div class="card" style="width: 18rem;">
                <img class="card-img-top" src="../assets/1648631992.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div>

               <div class="card" style="width: 18rem;">
                <img class="card-img-top" src="../assets/1648631992.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Card title</h5>
                  <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div> -->
      <TopProduct :product="product" v-for="product in products" :key="product.index" ></TopProduct>
     </div>
    
    </div>
  </div>
  
        
    
</template>

<script>
import TopProduct from './TopProduct.vue';
export default {
    name: 'TopProducts',

    data() {
        return {
            
        };
    },
    props:{
      products:Array
    },
    components:{
        TopProduct
    },


    methods: {
        
    },
};
</script>

<style  scoped>
    .display{
      /* width: 1200px; */
      display: flex;
      max-width: 1300px;
      min-width: 100px;
      margin: auto;
      /* border: 1px solid black; */
      flex-wrap: wrap;
    }
    .card{
      margin: 30px 10px 30px 10px;
      border-radius: 20px;
    }
    .row{
      border-radius: 10px;
      background: rgb(255, 230, 190);
      margin-bottom: 30px;
    }
</style>