<template>
  <div id="app">
    <div id = "tar-bar">
      <div class="tar-bar-item">主页</div>
      <div class="tar-bar-item">商品</div>
      <div class="tar-bar-item">购物车</div>
      <div class="tar-bar-item">我的</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  @import "./assets/css/base.css";
  #tar-bar{
    display: flex;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    background: #f1f1f1;
    box-shadow: 0px -1px 10px rgba(0 0 0 0.3)
  }
  .tar-bar-item{
    flex: 1;
    text-align: center;
    height: 49px;
  }


</style>
