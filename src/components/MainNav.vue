<template>
    <VueprojectNav></VueprojectNav>
   
   <div class="container">
        <div class="row" id="row">
                  <div class="col-sm-2">
                       <div style="padding:10px" class="logo">Lixibox</div>
                   </div>

              <div class="col-sm-7">
                  <div class="search-bar">
                          
                           <input style="padding: 10px; width: 100%; padding-right: 100px; border: 1px solid black; position: absolute;left: 0;" type="text" placeholder="Tìm kiếm">
                           <button style="padding: 10px;border: 1px solid black ;position: absolute;right: 0" class="btn-search"><i class="fa-solid fa-magnifying-glass fa-sm"></i>Tìm kiếm</button>
            
                  </div>
              </div>
                <div class="col-sm-2">
                           <div class="register" style="padding:10px">
                                 <a href="">Đăng nhập/</a>
                                     <a href="">Đăng kí</a>
                             </div>
                </div>
           <div class="col-sm-1">
                  <div class="cart" style="padding:10px">
                  <a href=""> <i class="fa-solid fa-cart-shopping fa-xl"></i> </a>
               
            </div>
           </div>
          
        </div>
          
    </div>
      
        <div class="line2">
            <div class="container">
                      <nav>
                <ul class="menu">
                    <li><a href="">  SHOP BEAUTY   </a></li>
                    <li><a href="">  SHOP MẸ VÀ BÉ  </a></li>
                    <li><a href="">  ƯU ĐÃI  </a></li>
                    <li><a href="">  THƯƠNG HIỆU  </a></li>
                    <li><a href="">  GIỚI THIỆU BẠN BÈ  </a></li>
                    <li><a href="">  MAGAZINE</a></li>
                    <li><a href=""> <i class="fa-brands fa-youtube fa-xl"></i> FEED  </a></li>

                </ul>

            </nav>
            </div>
          
        </div>
   
</template>

<script>
import VueprojectNav from './Nav.vue';
export default {
    name: 'MainNav',

    data() {
        return {
            
        };
    },
    components:{
        VueprojectNav
    }


};
</script>

<style  scoped>
    .logo{
        border: 1px solid black;
    }
   
    #row{
         padding: 30px 50px 30px 50px;
    }
    .search-bar{
         border: 1px solid black;
         position: relative;
    }
  
    
    .line2{
     
        padding: 30px 120px 30px 120px;
    }
    
    .menu{
        
        display: flex;
        justify-content: space-around;
    }
    
</style>