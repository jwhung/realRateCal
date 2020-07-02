<template>
	<view class="intro">
		<view class="title_area">
		  <text class="title">计算结果</text>
		  <text class="line"></text>
		</view>
		<view class="conclusion">{{conclusion}}</view>
		<view class="content">
		  <view class="item">{{fake}}%</view>
		  <view class="desc">名义利率</view>
		  <view class="line"></view>
		  <view class="item">{{real}}%</view>
		  <view class="desc">实际利率</view>
		</view>
	</view>
</template>

<script>
	export default {
		
	}
</script>

<style scoped>
.intro {
  margin: 0 10px;
}
.title_area{
  position: relative;
  display: inline-block;
  margin-bottom: 10px;
}
.title_area .title {
  font-size: 22px;
  color: #303133;
  position: relative;
  z-index: 999;
}
.title_area .line{
  width: 100%;
  height: 20rpx;
  background: #27C18F;
  opacity: 0.8;
  position: absolute;
  bottom: 0;
  z-index: 0;
  left: 0;
}
.content {
  font-size: 16px;
  color: #606266;
  margin-bottom: 10px; 
}
</style>