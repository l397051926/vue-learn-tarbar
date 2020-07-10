<template>
  <div class="tar-bar-item">
    <div v-if="!isActive"><slot name="item-img"></slot></div>
    <div v-else><slot name="item-img-active"></slot></div>
    <div :class="{active : isActive}"><slot name="item-text"></slot></div>
    <h2>{{isActive}}</h2>
  </div>
</template>

<script>
    export default {
        name: "TarbarItem",
        data(){
            return{
                isActive: false
            }
        }
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
  .active{
    color: red;
  }
</style>
