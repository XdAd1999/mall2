<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item path="/home" activeColor="pink">
        <img slot="item-icon" src="./assets/img/tabbar/shouye1.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/shouye_active.svg"
          alt=""
        />
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/cart" activeColor="pink">
        <img slot="item-icon" src="./assets/img/tabbar/fenlei.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/fenlei_active.svg"
          alt=""
        />
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/category" activeColor="pink">
        <img slot="item-icon" src="./assets/img/tabbar/gouwuche.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/gwca_active.svg"
          alt=""
        />
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile" activeColor="pink">
        <img slot="item-icon" src="./assets/img/tabbar/yonghu.svg" alt="" />
        <img
          slot="item-icon-active"
          src="./assets/img/tabbar/yonghu_active.svg"
          alt=""
        />
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/tabbar/TabBar";
import TabBarItem from "./components/tabbar/TabBarItem";
export default {
  name: "App",
  components: { TabBar, TabBarItem },
};
</script>

<style>
@import "./assets/css/tabbar.css";
</style>
