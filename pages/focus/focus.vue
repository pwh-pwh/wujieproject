<template>
	<view class="container">
		<view class="logo">
			<image src="/static/img/wujielogo.png"/>
		</view>
		<view style="text-align: center;font-size: medium;">Handpicked Experiences</view>
		<view style="text-align: center;font-size: small;">给你一个专属文化的世界</view>
		<view style="text-align: center;font-size: small;">以翻转模式构造传统文化新平台</view>
		 <button class="start" @click="toPath">立即体验</button> 
	</view>
</template>

<script>
	export default {
		data() {
			return {
			};
		},
		methods:{
			toPath(){
				uni.redirectTo({
					url:"../login/login"
				})
			}
		}
	}
</script>

<style lang="scss" scoped>
	.container{
		position:fixed;
		top:0;
		bottom:0;
		left:0;
		right:0;
			image{
				width: 100%;
				height: 100%;
			}
			.start{
				position: absolute;
				bottom:20upx;
				left:50%;
				transform: translate(-50%,-50%);
				border:1px solid #C0C0C0;
				background:rgba(255,255,255,0.5);
				border-radius: 4px;
				color:black;
			}
		
	}
	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 300rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: auto;
	}
</style>
