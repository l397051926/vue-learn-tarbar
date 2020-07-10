<template>
  <div id = "tar-bar">
    <slot></slot>
  </div>

</template>

<script>
    export default {
        name: "Tarbar",
        components:{

        }
    }
</script>

<style scoped>
  #tar-bar{
    display: flex;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    background: #f1f1f1;
    box-shadow: 0px -1px 10px rgba(0 0 0 0.3)
  }


</style>
