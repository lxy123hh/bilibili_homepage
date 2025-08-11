<script setup lang="ts">
import { Search } from '@element-plus/icons-vue'
import { GameThree, Mail } from '@icon-park/vue-next'
import { ref } from 'vue'

const input = ref('')
</script>

<template>
  <view class="TopNavBar">
    <!-- 上半部分 展示头像，输入框，两个icon -->
    <view class="TopNavBar-header">
      <view class="avatar-container">
        <el-avatar :size="50" src="/public/avatar.png" />
      </view>
      <el-input
        v-model="input"
        style="width: 240px"
        placeholder="Please Input"
        :prefix-icon="Search"
      />
      <view class="icons">
        <game-three theme="outline" size="24" fill="#333" :strokeWidth="2"/>
        <mail theme="outline" size="24" fill="#333" :strokeWidth="2"/>
      </view>
    </view>

    <!-- 下半部分 -->
    <view class="TopNavBar-menu">

    </view>
  </view>
</template>

<style scoped lang="scss">
.TopNavBar {
  height: 180rpx;
}
.TopNavBar-header {
  display: flex;
  height: 100rpx;
  align-items: center;
  padding: 20rpx 20rpx;
  justify-content: space-between;
}
.icons {
  display: flex;
  gap: 5rpx;
}

</style>
