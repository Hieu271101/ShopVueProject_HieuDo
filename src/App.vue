<template>
    <div>
      
      <MainNav></MainNav>
     
      <BodyVue :topProductList="topProductList" :products="listProducts"></BodyVue>
    
     <RegisterForm></RegisterForm>
    <OrderCheck></OrderCheck>
    <ShopsVue :shops="listShop"></ShopsVue>

    <Cart></Cart>
     <VueprojectFooter></VueprojectFooter>

    </div>
</template>

<script>

import MainNav from './components/MainNav.vue'
// import TopProducts from './components/TopProducts.vue'
// import MainProductsVue from './components/MainProducts.vue'
import VueprojectFooter from './components/Footer.vue'
// import VueprojectFilter from './components/Filter.vue'
import RegisterForm from './components/RegisterForm.vue'

import BodyVue from './components/Body.vue'

import OrderCheck from './components/OrderCheck.vue'

import ShopsVue from './components/Shops.vue'

import Cart from './components/Cart.vue'
export default {
  name: 'App',
  components: {
    MainNav,
    // TopProducts,
    // MainProductsVue,
    VueprojectFooter,
    // VueprojectFilter,
    RegisterForm,
    BodyVue,
    OrderCheck,
    ShopsVue,
    Cart
},
  data() {
    return {
      listShop:[],
      listProducts:[],
      topProductList:[]
    }
  },
  created(){
    this.listShop=[
      {
        img:'https://upload.lixibox.com/system/store/information/images/000/000/001/original/1649237668.jpeg',
        name:'Phạm Ngọc Thạch',
        address: '16 Phạm Ngọc Thạch, phường 6, quận 3, TP.HCM',
        hotline:'02838293052',
        email:'phamngocthach.store@lixibox.com',
        workingTime:'Tất cả các ngày trong tuần',
        openingTime:'08:30 - 21:30'
      },
       {
        img:'https://upload.lixibox.com/system/store/information/images/000/000/001/original/1649237668.jpeg',
        name:'Phạm Ngọc Thạch',
        address: '16 Phạm Ngọc Thạch, phường 6, quận 3, TP.HCM',
        hotline:'02838293052',
        email:'phamngocthach.store@lixibox.com',
        workingTime:'Tất cả các ngày trong tuần',
        openingTime:'08:30 - 21:30'
      },
     
    ],

    this.listProducts=[
      {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
         {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
        {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
        {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
        {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
        {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
    ],
   
   this.topProductList=[
      {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
       {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
       {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
       {
        img:'https://upload.lixibox.com/system/pictures/files/000/073/261/square/1654829019.jpg?t=1656905522 ',
        title:'Kiin',
        description:'Gel Bôi Sát Khuẩn Vùng Nướu Dành Cho Răng Viêm Nha Chu Loét Miệng PERIO KIN 30ml',
        price:'126.000 đ',
      },
      
    ]
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
}
</style>
