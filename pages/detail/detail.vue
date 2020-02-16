<template>
	<view class="content">
		<view class="tabbar">
			<view class="tab hl">产品详情<view class="line"></view></view>
			<view class="tab">使用说明<view class="line"></view></view>
		</view>
		<scroll-view class="scroll">
			<swiper class="swiper" :indicator-dots="true" :autoplay="true">
				<swiper-item>
				   <image class="point" src="/static/logo.png"></image>
				</swiper-item>
				<swiper-item>
				   <image class="point" src="/static/logo.png"></image>
				</swiper-item>
				<swiper-item>
				   <image class="point" src="/static/logo.png"></image>
				</swiper-item>
				<swiper-item>
				   <image class="point" src="/static/logo.png"></image>
				</swiper-item>
				<swiper-item>
				   <image class="point" src="/static/logo.png"></image>
				</swiper-item>
			</swiper>
			<view class="timeFrame">
				<view class="time">限时抢购</view>
				<view class="time">已结束</view>
			</view>
			<view class="mainFrame">
				<view class="title">
					库存告急！中午12点准时下架！【全国京东物流包邮72小时内发货】原森态更好的防护~199元抢门市价399元原生态防雾霾PM2.5
				防尘防病菌KN95透气电动防护口罩~手慢无~
				</view>
				<view class="price"><text style="font-size: 26rpx;">&yen;</text>199</view>
				<view class="fan">
					<view class="left">超返</view>
					<view class="right">&yen;20</view>
				</view>
				<view class="number">已售:821 库存:73</view>
			</view>
		</scroll-view>
		<view class="bottom">
			<view class="index" @click="goHome">首页</view>
			<view class="button">分享</view>
			<view class="button">抢购</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		},
		methods:{
			goHome(){
				uni.reLaunch({
					url:'/pages/index/index'
				})
			}
		}
	}
</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		position:fixed;
		top:0;
		left:0;
		right:0;
		bottom:0;
		background-color: #f3f2f2;
		.tabbar{
			width:750rpx;
			height: 88rpx;
			background-color:#fff;
			display: flex;
			flex-shrink: 0;
			.tab{
				width:50%;
				height: 100%;
				position: relative;
				line-height: 88rpx;
				font-size: 28rpx;
				text-align: center;
				.line{
					width:10%;
					height: 2px;
					position: absolute;
					left: 45%;
					bottom:2rpx;
					background-color:#f8ab0c;
					display: none;
				}
				&.hl{
					font-weight: bolder;
					.line{display: block;}
				}
			}
		}
		.scroll{
			width: 750rpx;
			height: 10px;
			flex-grow: 1;
			overflow: hidden;
			.swiper{
				width:750rpx;
				height: 346rpx;
				.point{
					width:750rpx;
					height: 346rpx;
				}
			}
			.timeFrame{
				width:750rpx;
				height: 86rpx;
				background-color: #fd3f6b;
				display: flex;
				align-items: center;
				justify-content: space-between;
				padding: 0 22rpx;
				.time{
					font-size: 28rpx;
					color: #fff;
				}
			}
			.mainFrame{
				width: 100%;
				padding: 32rpx 30rpx 50rpx 20rpx;
				background-color: #fff;
				.title{
					font-size: 28rpx;
					line-height: 1.5;
				}
				.price{
					font-size: 32rpx;
					color: #f46838;
					margin-top: 50rpx;
				}
				.fan{
					height: 37rpx;
					padding: 4rpx;
					background-color: #f46838;
					display: flex;
					align-items: center;
					border-radius: 6rpx;
					width: fit-content;
					margin-top: 30rpx;
					.left{
						padding: 0 5rpx;
						font-size: 22rpx;
						color: #fff;
						line-height: 29rpx;
						flex-shrink: 0;
					}
					.right{
						padding: 0 5rpx;
						font-size: 22rpx;
						color: #f46838;
						line-height: 29rpx;
						flex-shrink: 0;
						background-color: #fff;
					}
				}
				.number{
					font-size: 23rpx;
					color: #aaa;
					text-align: right;
					margin-top: 38rpx;
				}
			}
		}
		.bottom{
			width: 750rpx;
			height: 80rpx;
			flex-shrink: 0;
			display: flex;
			align-items: center;
			justify-content: space-between;
			.index{
				width:30%;
				height: 80rpx;
				line-height: 80rpx;
				text-align: center;
				font-size: 42rpx;
				border: 1px solid #e2c168;
				background-color: #fff;
			}
			.button{
				width:35%;
				height: 80rpx;
				line-height: 80rpx;
				text-align: center;
				font-size: 42rpx;
				background-color: #ff0000;
				color: #fff;
				border: 1px solid #e2c168;
				border-left: 0;
			}
		}
	}
</style>
