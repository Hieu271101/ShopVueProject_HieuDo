<template>
    <div>
         <div class="card" style="width: 18rem;">
                <img class="card-img-top" :src=product.img alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">{{product.title}}</h5>
                  <p class="card-text">{{product.description}}</p>
                  <p>{{product.price}}</p>
                 <a href="" class="btn btn-primary">Đi đến giỏ hàng</a>
              </div>
           </div>
    </div>
</template>

<script>
export default {
    name: 'TopProduct',

    data() {
        return {
            
        };
    },
    props:{
        product:Object
    },
   
    methods: {
        
    },
};
</script>

<style scoped>
     .card{
      margin: 30px 10px 30px 10px;
      border-radius: 20px;
    }
</style>