<template>
  <view class="container">
    <text class="title">欢迎来到首页</text>
    <button class="blockly-btn" type="primary" @click="openBlocklyEditor">
      打开 Blockly 编辑器
    </button>
  </view>
</template>

<script>
export default {
  methods: {
    openBlocklyEditor() {
      // 使用 uni.navigateTo 跳转到 Blockly 页面
      uni.navigateTo({
        url: '/pages/blockly/blockly'
      });
    }
  }
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
.title {
  font-size: 20px;
  color: #333;
  margin-bottom: 20rpx;
}
.blockly-btn {
  margin: 20rpx;
  padding: 20rpx;
  background-color: #27ae60;
  color: #fff;
  border-radius: 10rpx;
}
</style>
