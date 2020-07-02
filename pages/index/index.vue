<template>
	<view class="card">
	  <form catchsubmit="formSubmit" catchreset="formReset">
	    <view class="items">
	      <text class="item">金额</text><input type="digit" name="bj" placeholder="请输入分期/借款的金额" value="10000" />
	    </view>
	    <view class="items">
	      <text class="item">期数</text><input type="number" name="qs" placeholder="请输入分期/借款的期数"  value="12"/>
	    </view>
	    <view class="items">
	      <text class="item">一次性手续费</text><input type="digit" name="ycxsxf" placeholder="借款时一次性交的手续费" value="0"/>
	    </view>
	    <view class="items">
	      <text class="item">每期手续费</text><input type="digit" name="mqsxf" placeholder="每期需要交的手续费" value="100" />
	    </view>
	    <view class="area">       
	      <button class="button main" type="default" size="mini" form-type="submit"> 立即计算 </button>        
	      <button class="button" type="default" size="mini" form-type="reset"> 清空内容 </button>
	    </view>
	    <view>{{tips}}</view>
	  </form>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				href: 'https://uniapp.dcloud.io/component/README?id=uniui'
			}
		},
		methods: {

		}
	}
</script>

<style>
.card {
	padding: 20px;
	font-size: 14px;
	line-height: 24px;
}
.intro {
	margin: 10px;
	text-align: center;
}
.items {
	padding: 5px;
	color: #606266;
	text-align: left;
}
.item {
    font-size: 18px;
}
input {
	width: 100%;
	float: left;
	height: 40px;
	border: 1px solid #27C18F;
	margin: 0 auto 10px;
	border-radius: 4px;
	color: #333333;
	text-align: center;
}
.area{
	margin-top: 50px;
}
.area .button {
	width: 98%;
	height: 50px;
	font-size: 18px;
	text-align: center;
	color: #27C18F;
	background-color: #fff;
	border: 1px solid #27C18F;
	margin: 5px;
	float: left;
	padding: 5px;
}
.area .main{
	background-color: #27C18F !important;
	color: #fff;
}
</style>
