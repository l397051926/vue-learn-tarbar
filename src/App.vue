<template>
  <div id="app">
    <router-view></router-view>
    <tarbar>
      <tabBariItem path="/home" activeColor="blue">
        <img slot="item-img" src="@/assets/image/home.svg"/>
        <img slot="item-img-active" src="@/assets/image/home-active.svg"/>
        <div slot="item-text">主页</div>
      </tabBariItem>
      <tabBariItem path="/category">
        <img slot="item-img" src="@/assets/image/category.svg"/>
        <img slot="item-img-active" src="@/assets/image/category-active.svg"/>
        <div slot="item-text">分类</div>
      </tabBariItem>
      <tabBariItem path="/cart">
        <img slot="item-img" src="@/assets/image/cart.svg"/>
        <img slot="item-img-active" src="@/assets/image/cart-active.svg"/>
        <div slot="item-text">购物车</div>
      </tabBariItem>
      <tabBariItem path="/profile">
        <img slot="item-img" src="@/assets/image/profile.svg"/>
        <img slot="item-img-active" src="@/assets/image/profile-active.svg"/>
        <div slot="item-text">我的</div>
      </tabBariItem>
    </tarbar>
  </div>
</template>

<script>
  import tarbar from "./components/tarbar/Tarbar"
  import tabBariItem from "./components/tarbar/TarbarItem"

  export default {
  name: 'App',
      components:{
          tarbar ,
          tabBariItem
      }
}
</script>

<style>
  @import "./assets/css/base.css";

</style>
