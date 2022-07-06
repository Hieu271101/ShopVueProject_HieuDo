<template>
    <div>
        <div class="cover">
            <div class="box">
                <label for=""><h1>Danh sách cửa hàng</h1></label>
                <div style="display: flex">
                    <input type="text" placeholder="nhập địa chỉ cửa hàng hoặc tên cửa hàng" style="padding:10px; font-size:15px; width:500px"> <button type="button" style="width:50px; background-color:pink; padding:10px"><i class="fa-solid fa-magnifying-glass"></i></button>
                </div>
            </div>
        </div>
    <div style="padding: 30px 50px 30px 50px">
        <div class="grid  grid-cols-2">
            <!-- <div class="item">
                <div>
                    <img style="width:100%" src="https://upload.lixibox.com/system/store/information/images/000/000/001/original/1649237668.jpeg" alt="">
                </div>
              
                <div class="information-form">
                    <div>
                         <label for="">Phạm Ngọc Thạch</label>
                    </div>
                   <div>
                        <i class="fa-solid fa-location-dot"></i> 16 Phạm Ngọc Thạch, phường 6, quận 3, TP.HCM <a href="">Xem bản đồ</a>
                   </div>
                   <div>
                      <i class="fa-solid fa-phone"></i> Hotline: 02838293052 
                   </div>
                   <div>
                        <i class="fa-solid fa-envelope"></i> phamngocthach.store@lixibox.com
                   </div>
                   <div>
                        <i class="fa-solid fa-calendar-days"></i> Thời gian hoạt động: Tất cả các ngày trong tuần
                   </div>
                   <div>
                        <i class="fa-solid fa-clock"></i> Giờ mở cửa: 08:30 - 21:30
                   </div>
                    
                </div>
            </div>
             <div class="item">02</div>
             <div class="item">03</div>
              <div class="item">04</div> -->
           <ShopVue :shop="shop" v-for=" shop in shops" :key="shop.index"> </ShopVue>     
        </div>
    </div>
       
    </div>
</template>

<script>
    import  ShopVue  from "../components/Shop.vue";
export default {
    
    name: 'ShopsVue',

    data() {
        return {
            
        };
    },
    components:{
        ShopVue
    },

   props:{
        shops:Array
   },

    methods: {
        
    },
};
</script>

<style  scoped>
    .cover{
          height: 300px;
          padding: 20px;
          margin-bottom: 40px;
        background-image: url(../assets/cover.png);
        background-size: cover;
        background-position: center;
       
        display: flex;
        flex-direction: column;

        justify-content: center;
        align-items: center;
        text-align: center;
    }
    .box{
         font-size: 25px;
          line-height: 25px;
        margin-bottom: 20px;
    }
    .information-form{
        padding: 10px;
        /* border: 1px solid black; */
        width: 85%;
        margin: 0 25px;
        box-shadow: 0 4px 4px rgb(0 0 0 / 25%);
         border-radius: 8px;
    }
    .item{
        margin: 25px;
    }
</style>