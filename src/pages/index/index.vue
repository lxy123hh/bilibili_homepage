<!-- 使用 type="home" 属性设置首页，其他页面不需要设置，默认为page -->
<route lang="jsonc" type="home">
{
  "layout": "tabbar",
  "style": {
    // 'custom' 表示开启自定义导航栏，默认 'default'
    "navigationStyle": "custom",
    "navigationBarTitleText": "首页"
  }
}
</route>

<script lang="ts" setup>
import BottonTabBar from '@/components/layout/BottonTabBar.vue'
import HomePage from '@/components/layout/HomeMain.vue'
import TopNavBar from '@/components/layout/TopNavBar.vue'
</script>

<template>
  <view class="index">
    <TopNavBar />
    <HomePage />
    <BottonTabBar />
  </view>
</template>

<style scoped>
.index {
  min-height: 100vh;
  background-color: #ffffff;
  display: flex;
  flex-direction: column;
}
</style>
