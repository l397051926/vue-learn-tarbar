<template>
  <div id="app">
    <router-view></router-view>
    <main-tarbar></main-tarbar>
  </div>
</template>

<script>

  import mainTarbar from "./components/MainTarbar"

  export default {
  name: 'App',
      components:{
          mainTarbar
      }
}
</script>

<style>
  @import "./assets/css/base.css";

</style>
