<template>
	<view class="content">
		<view class="head">
			<view class="back"></view>
			<view class="search"></view>
		</view>
		<scroll-view scroll-x="true" class="tabbar">
			<view class="tabFrame">
				<view class="tab hl">精选<view class="line"></view></view>
				<view class="tab">家居用品<view class="line"></view></view>
				<view class="tab">食品饮料<view class="line"></view></view>
				<view class="tab">母婴<view class="line"></view></view>
				<view class="tab">美妆护肤<view class="line"></view></view>
				<view class="tab">猫猫狗狗<view class="line"></view></view>
				<view class="tab">鱼虾蟹<view class="line"></view></view>
			</view>
		</scroll-view>
		<scroll-view scroll-y="true" class="bottom">
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
			<view class="point" @click="goDetail">
				<image class="pic" src="/static/logo.png"></image>
				<view class="right">
					<view class="pointTop">
						<view class="title">
							<image src="/static/1.png" class="jd"></image>
							<text>[抢！拍3件仅199元] 味库 越南活冻...</text>
						</view>
						<image class="smallShare" src="/static/2.png"></image>
					</view>
					<view class="pointBottom">
						<view class="priceFrame">
							<view class="price">&yen;<text style="font-size: 28rpx;">85</text> 抢购</view>
							<view class="other">
								<view class="coupon">3元券</view>
								<view class="earn">赚 &yen;0.9</view>
							</view>
						</view>
						<image class="bigShare" src="/static/3.png"></image>
					</view>
				</view>
			</view>
		</scroll-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {
			goDetail(){
				uni.navigateTo({
					url:'/pages/detail/detail'
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
		.head{
			width:750rpx;
			height:75rpx;
			background-image: url('~@/static/0.png');
			background-size: 750rpx 75rpx;
			position: relative;
			flex-shrink: 0;
			.back{
				width:25rpx;
				height:30rpx;
				position: absolute;
				top:23rpx;
				left:33rpx;
			}
			.search{
				width:33rpx;
				height:30rpx;
				position: absolute;
				top:23rpx;
				right:27rpx;
			}
		}
		.tabbar{
			width:750rpx;
			height: 64rpx;
			background-color: #fff;
			flex-shrink: 0;
			overflow: hidden;
			.tabFrame{
				height: 64rpx;
				display: flex;
				flex-wrap: nowrap;
				align-items: center;
				padding: 0 37rpx;
				.tab{
					font-size: 24rpx;
					padding: 0 37rpx;
					flex-shrink: 0;
					position: relative;
					.line{
						width:100%;
						height: 2rpx;
						background-color: #333;
						position: absolute;
						bottom:-9rpx;
						left:0rpx;
						display: none;
					}
					&.hl{
						font-weight: bold;
						.line{
							display:block;
						}
					}
				}
			}
		}
		.bottom{
			width:750rpx;
			height: 10px;
			flex-grow: 1;
			background-color: #f2f1f5;
			padding-top: 8rpx;
			.point{
				height:227rpx;
				width:703rpx;
				background-color: #fff;
				border-radius: 10rpx;
				margin: auto;
				margin-bottom: 17rpx;
				padding: 5rpx 0 5rpx 17rpx;
				display: flex;
				align-items: center;
				justify-content: space-between;
				.pic{
					width:217rpx;
					height:217rpx;
					flex-shrink: 0;
				}
				.right{
					width:403rpx;
					height: 100%;
					display: flex;
					flex-direction: column;
					justify-content: space-between;
					.pointTop{
						width:100%;
						display: flex;
						align-items: center;
						justify-content: space-between;
						padding-top: 14rpx;
						.title{
							width:260rpx;
							font-size: 23rpx;
							line-height: 1.5;
							.jd{
								width:29rpx;
								height:26rpx;
								margin-right: 20rpx;
							}
						}
						.smallShare{
							width:101rpx;
							height:34rpx;
						}
					}
					.pointBottom{
						display: flex;
						justify-content: space-between;
						align-items: center;
						.priceFrame{
							.price{
								font-size: 18rpx;
								color: red;
							}
							.other{
								display: flex;
								align-items: center;
								.coupon{
									width:128rpx;
									height: 30rpx;
									margin-right: 10rpx;
									background-size: 128rpx 30rpx;
									line-height: 30rpx;
									text-align: center;
									font-size: 20rpx;
									color: #fff;
									background-image: url('~@/static/4.png');
								}
								.earn{
									padding: 3rpx 18rpx;
									background-color: #feecc5;
									font-size: 18rpx;
									color: #75512a;
								}
							}
						}
						.bigShare{
							width:127rpx;
							height:74rpx;
						}
					}
				}
			}
		}
	}
</style>
