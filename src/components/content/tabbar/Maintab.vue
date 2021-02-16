<template>
  <div>
      <tab-bar>
      <tab-bar-item path="/home" stylecolor="red">
        <img slot="tab-item-img" src="../../assets/img/index.png" alt="">
        <img slot="tab-item-ing" src="../../assets/img/index_blue.png" alt="">
        <div slot="tab-item-div">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/others" stylecolor="red">
        <img slot="tab-item-img" src="../../assets/img/index.png" alt="">
        <img slot="tab-item-ing" src="../../assets/img/index_blue.png" alt="">
        <div slot="tab-item-div">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/shopcar" stylecolor="red">
        <img slot="tab-item-img" src="../../assets/img/index.png" alt="">
        <img slot="tab-item-ing" src="../../assets/img/index_blue.png" alt="">
        <div slot="tab-item-div">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/mine" stylecolor="red">
        <img slot="tab-item-img" src="../../assets/img/index.png" alt="">
        <img slot="tab-item-ing" src="../../assets/img/index_blue.png" alt="">
        <div slot="tab-item-div">我的</div>
      </tab-bar-item>
      </tab-bar> 
  </div>
</template>

<script>

 import TabBar from './TabBar.vue'
 import TabBarItem from './TabBarItem.vue'

export default {
    components:{
      TabBar,
    TabBarItem
    }
};
</script>
<style >
 @import url(../../assets/css/tabbar.css);
</style>