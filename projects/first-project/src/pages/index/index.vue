<template>
  <view class="index">
    <view class="global-image">
      <view class="title">全局目录图片</view>
      <image class="icon-global-image" src="@global/assets/imgs/icon_global_logo.png" />
    </view>
    <view class="src-image">
      <view class="title">src目录图片</view>
      <image class="icon-src-image" src="@/assets/imgs/icon_logo.png" />
    </view>
    <view>
      <global-component />
    </view>
    <view>
      <src-component />
    </view>
  </view>
</template>

<script setup>
import GlobalComponent from '@global/components/global-component.vue'
import SrcComponent from '@/components/src-component.vue'
</script>

<style lang="scss">
.index {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100vh;
  .global-image, .src-image {
    text-align: center;
    .title {
      margin-bottom: 24px;
    }
  }
  .icon-global-image {
    width: 109px;
    height: 109px;
  }
  .icon-src-image {
    width: 218px;
    height: 186px;
  }
}
</style>
