<template>
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
</template>

<script>
    import tarbar from "./tarbar/Tarbar"
    import tabBariItem from "./tarbar/TarbarItem"

    export default {
        name: "MainTarbar",
        data() {
            return {
                // tarbarItems:[
                //     {
                //         name: "主页",
                //         path: "/home",
                //         itemImg: "@/assets/image/home.svg",
                //         itemImgActive: "@/assets/image/home-active.svg"
                //     },
                //     {
                //         name: "分类",
                //         path: "/category",
                //         itemImg: "@/assets/image/category.svg",
                //         itemImgActive: "@/assets/image/category-active.svg"
                //     },
                //     {
                //         name: "购物车",
                //         path: "/cart",
                //         itemImg: "@/assets/image/cart.svg",
                //         itemImgActive: "@/assets/image/cart-active.svg"
                //     },
                //     {
                //         name: "我的",
                //         path: "/profile",
                //         itemImg: "@/assets/image/profile.svg",
                //         itemImgActive: "@/assets/image/profile-active.svg"
                //     }
                // ]
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
