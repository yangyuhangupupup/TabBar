<template>
       <tab-bar>
    <tab-bar-item path="/home">
      <img slot="icon-image"
           src="../../assets/image/home.svg"
           alt="">
      <img slot="active-image"
           src="../../assets/image/homes.svg"
           alt="">
      <div slot="icon-text">首页</div>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <img slot="icon-image"
           src="../../assets/image/fenlei.svg"
           alt="">
      <img slot="active-image"
           src="../../assets/image/fenleis.svg"
           alt="">
      <div slot="icon-text">分类</div>
    </tab-bar-item>
    <tab-bar-item path="/shopcar">
      <img slot="icon-image"
           src="../../assets/image/car.svg"
           alt="">
      <img slot="active-image"
           src="../../assets/image/cars.svg"
           alt="">
      <div slot="icon-text">购物车</div>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <img slot="icon-image"
           src="../../assets/image/my.svg"
           alt="">
      <img slot="active-image"
           src="../../assets/image/mys.svg"
           alt="">
      <div slot="icon-text">我的</div>
    </tab-bar-item>
  </tab-bar>
</template>
<script>
import TabBar from './Tabbar'
import TabBarItem from './TabarItem'
export default {
  name: '',
  data () {
    return {};
  },
  computed: {},
  created () { },
  mounted () { },
  methods: {},
  components: {
    TabBar,
    TabBarItem
  }
};
</script>
<style scoped >
</style>
