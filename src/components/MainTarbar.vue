<template>
  <tarbar >
    <tabBariItem v-for="(item, index) in tarbarItems" :path="item.path">
      <img slot="item-img" :src="item.itemImg"/>
      <img slot="item-img-active" :src="item.itemImgActive"/>
      <div slot="item-text">{{item.name}}</div>
    </tabBariItem>
  </tarbar>
</template>

<script>
    import tarbar from "./tarbar/Tarbar"
    import tabBariItem from "./tarbar/TarbarItem"

    export default {
        name: "MainTarbar",
        data() {
            return {
                tarbarItems:[
                    {
                        name: "主页",
                        path: "/home",
                        itemImg: "@/assets/image/home.svg",
                        itemImgActive: "@/assets/image/home-active.svg"
                    },
                    {
                        name: "分类",
                        path: "/category",
                        itemImg: "@/assets/image/category.svg",
                        itemImgActive: "@/assets/image/category-active.svg"
                    },
                    {
                        name: "购物车",
                        path: "/cart",
                        itemImg: "@/assets/image/cart.svg",
                        itemImgActive: "@/assets/image/cart-active.svg"
                    },
                    {
                        name: "我的",
                        path: "/profile",
                        itemImg: "@/assets/image/profile.svg",
                        itemImgActive: "@/assets/image/profile-active.svg"
                    }
                ]
            }
        },
        components: {
            tarbar,
            tabBariItem
        }
    }
</script>

<style scoped>

</style>
