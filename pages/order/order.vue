<template>
	<view class="content">
		<view class="tabbar">
			<view class="tab" :class="{hl:!item}" @click="changeItem(0)">京东订单</view>
			<view class="tab" :class="{hl:item}" style="border-left: 0;" @click="changeItem(1)">返佣</view>
		</view>
		<scroll-view scroll-y="true" class="scroll">
			<block v-if="!item">
				<view class="point">
					<view class="top">
						<view class="left">[全国京东物流包邮·72小时内发货]原森态更好的防护~199元抢门市价399元原森态防雾霾PM2.5防尘防病菌KN...</view>
						<view class="right">40.00</view>
					</view>
					<view class="bottom">
						2020-01-00 21:15:58
					</view>
				</view>
				<view class="point">
					<view class="top">
						<view class="left">[全国京东物流包邮·72小时内发货]原森态更好的防护~199元抢门市价399元原森态防雾霾PM2.5防尘防病菌KN...</view>
						<view class="right">40.00</view>
					</view>
					<view class="bottom">
						2020-01-00 21:15:58
					</view>
				</view>
				<view class="point">
					<view class="top">
						<view class="left">[全国京东物流包邮·72小时内发货]原森态更好的防护~199元抢门市价399元原森态防雾霾PM2.5防尘防病菌KN...</view>
						<view class="right">40.00</view>
					</view>
					<view class="bottom">
						2020-01-00 21:15:58
					</view>
				</view>
			</block>
			<view class="rebatFrame" v-else>
				<view class="rebatTitle">最近3次京东返佣入账记录</view>
				<view class="rebatDsc">(京东返佣，每月10号自动入账“可提现余额”)</view>
				<view class="rebat">2020-01-02&nbsp;16:51:21&nbsp;&nbsp;&nbsp;&yen;&nbsp;2941.69</view>
				<view class="rebat">2020-01-02&nbsp;16:51:21&nbsp;&nbsp;&nbsp;&yen;&nbsp;2941.69</view>
				<view class="rebat">2020-01-02&nbsp;16:51:21&nbsp;&nbsp;&nbsp;&yen;&nbsp;2941.69</view>
			</view>
			
		</scroll-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				item:0
			};
		},
		methods:{
			changeItem(i){
				this.item=i
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
			height: 84rpx;
			display: flex;
			flex-shrink: 0;
			.tab{
				width:50%;
				background-color: #fff;
				line-height: 82rpx;
				text-align: center;
				font-size: 40rpx;
				border: 1px solid #e58d3e;
				&.hl{
					background-color: #bee6fb;
				}
			}
		}
		.scroll{
			width:750rpx;
			height:10px;
			flex-grow: 1;
			overflow: hidden;
			.point{
				width: 750rpx;
				height: 114rpx;
				background-color: #fff;
				padding: 17rpx 25rpx 24rpx 5rpx;
				display: flex;
				flex-direction: column;
				justify-content: space-between;
				border-bottom: 1px solid #ddd;
				.top{
					width:100%;
					height: 52rpx;
					display: flex;
					justify-content: space-between;
					align-items: center;
					.left{
						width: 640rpx;
						flex-shrink: 0;
						font-size: 23rpx;
						line-height: 1.5;
						transform: scale(0.8);
						transform-origin: left top;
						font-weight: bolder;
					}
					.right{
						font-size: 20rpx;
						line-height: 1;
					}
				}
				.bottom{
					font-size: 15rpx;
					color: #808080;
					transform: scale(0.9);
					transform-origin: left bottom;
				}
			}
			.rebatFrame{
				width: 750rpx;
				background-color: #fff;
			}
			.rebatTitle{
				padding-top: 29rpx;
				padding-left: 22rpx;
				font-size: 40rpx;
			}
			.rebatDsc{
				font-size: 28rpx;
				padding-left: 42rpx;
				margin-top: 9rpx;
			}
			.rebat{
				font-size: 31rpx;
				margin-top: 58rpx;
				padding-left: 15rpx;
			}
		}
		}
</style>
