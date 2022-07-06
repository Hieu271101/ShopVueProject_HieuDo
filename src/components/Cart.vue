<template>
    <div>
        <div class="content">
            <div class="left">
                <img style="width:100%" src="https://upload.lixibox.com/system/pictures/files/000/073/261/large/1654829019.jpg?v=2" alt="">
            </div>
            <div class="right">
               <div class="box1">
                     <div> <label for="">Ten</label></div>
                     <div style="font-size:30px; font-weight: bold;">description</div>
                     <div style="font-size:25px">Price</div>
               </div>

               <div class="box2">
                    <div class="item">
                        <div><i class="fa-brands fa-bitcoin fa-2xl"></i></div>
                        <div>Nhận ngay 126 Lixicoin khi mua sản phẩm này</div>
                    </div>
                    <div class="item">
                        <div><i class="fa-solid fa-van-shuttle fa-2xl"></i></div>
                        <div>Miễn phí giao hàng tối đa 15K cho đơn hàng từ 500K</div>
                    </div>
                    <div class="item">
                        <div><i class="fa-solid fa-rotate-left fa-2xl"></i></div>
                        <div>Đổi trả hàng trong 7 ngày</div>
                    </div>
                    
               </div>

               <div class="box4">
                    <button type="button" style="background: rgb(222, 50, 50); padding: 10px; width: 200px; border-radius: 8px;color: white;" >Thêm vào giỏ</button>
                    <button type="button" style="padding: 10px; width: 200px; border-radius: 8px; border:1px solid black">Yêu thích</button>
               </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CartVue',

    data() {
        return {
            
        };
    },

 
    methods: {
        
    },
};
</script>

<style  scoped>
    .content{
        
    display: flex;
    width: 100%;
    max-width: 1170px;
    margin: 0px auto;
    padding: 40px 0px 0px;
    justify-content: space-between;
    }
    .left{
        /* border: 1px solid black; */
        width: 60%;
        padding: 80px ;
        padding-top: 0;
        /* padding-right: 70px; */
     
    }
    .right{
        /* border: 1px solid black; */
        width: 40%;
    }
    .box1{
        line-height: 50px;
    }
    .box2{
        display: flex;
        /* border: 1px solid black; */
        width: 100%;
    
        flex-wrap: wrap;
        justify-content: space-between;
    }
    .item{
        width: 150px;
        /* border: 1px solid black; */
        padding: 10px;
        text-align: center;
        line-height: 35px;
        font-size: 15px;
    }
    .box4{
        display: flex;
        justify-content: space-around;
        width: 100%;
        padding: 10px;
    }

</style>