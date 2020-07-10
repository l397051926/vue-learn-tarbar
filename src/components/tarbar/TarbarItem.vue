<template>
  <div class="tar-bar-item">
    <slot name="item-img"></slot>
    <slot name="item-text"></slot>
  </div>
</template>

<script>
    export default {
        name: "TarbarItem"
    }
</script>

<style scoped>
  .tar-bar-item{
    flex: 1;
    text-align: center;
    height: 49px;
    font-size: 14px;
  }
  .tar-bar-item img{
    height: 25px;
    width: 25px;
    margin-top: 3px;
    vertical-align: middle;
    margin-bottom: 2px;
  }
</style>
