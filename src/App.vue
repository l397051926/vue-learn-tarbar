<template>
  <div id="app">
    <tarbar>
      <tabBariItem>
        <img slot="item-img" src="@/assets/image/home.svg"/>
        <img slot="item-img-active" src="@/assets/image/home-active.svg"/>
        <div slot="item-text">主页</div>
      </tabBariItem>
      <tabBariItem>
        <img slot="item-img" src="@/assets/image/all.svg"/>
        <img slot="item-img-active" src="@/assets/image/all-active.svg"/>
        <div slot="item-text">分类</div>
      </tabBariItem>
      <tabBariItem>
        <img slot="item-img" src="@/assets/image/cat.svg"/>
        <img slot="item-img-active" src="@/assets/image/cat-active.svg"/>
        <div slot="item-text">购物车</div>
      </tabBariItem>
      <tabBariItem>
        <img slot="item-img" src="@/assets/image/project-file.svg"/>
        <img slot="item-img-active" src="@/assets/image/project-file-active.svg"/>
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
