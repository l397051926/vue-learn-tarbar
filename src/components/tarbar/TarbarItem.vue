<template>
  <div class="tar-bar-item" @click="itemClick">
    <div v-if="!isActive"><slot name="item-img"></slot></div>
    <div v-else><slot name="item-img-active"></slot></div>
    <div :style="activeStyle" ><slot name="item-text"></slot></div>
  </div>
</template>

<script>
    export default {
        name: "TarbarItem",
        props: {
            path: String,
            activeColor :{
                type: String,
                default: "red"
            }
        },
        data(){
            return{
                // isActive: false
            }
        },
        computed:{
            isActive (){
                return this.$route.path.includes(this.path)
            },
            activeStyle(){
                return this.isActive ? {color: this.activeColor} : {}
            }
        },
        methods:{
            itemClick(){
                this.$router.replace(this.path)
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
