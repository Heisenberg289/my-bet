<template>
	<view class="content">
		<view class="top-box">
			<view class="top-logo"></view>
			<view class="top-title">
				<view class="line"></view>
				<view class="title">赞助伙伴</view>
				<view class="line"></view>
			</view>
			<view class="bottom-logo">
				<view class="left">
					<img src="/static/image-3.png" class="logo"/>
				</view>
				<view class="right">
					<img src="/static/image-4.png" class="logo"/>
				</view>
			</view>
		</view>
		<view class="login-box">
			<view class="login-inner">
				<view class="login-left">
					<view class="top-login">登陆</view>
					<view class="form">
						<view class="input-box">
							<view class="input">
								<view class="input-left"></view>
								<view class="input-middle">
									<input placeholder="4-11位字母或数字的用户名" maxlength="11" class="input-1"/>
								</view>
								<view class="input-right"></view>
							</view>
						</view>
						<view class="input-box">
							<view class="input">
								<view class="input-left input-left2"></view>
								<view class="input-middle">
									<input placeholder="6-12位字母或数字的密码" maxlength="11" class="input-1" stype="text"/>
								</view>
								<view class="input-right3"></view>
								<view class="input-right input-right2"></view>
							</view>
						</view>
					</view>
					<view class="other-opera">
						<view class="other-opera-1">
							<view class="other-opera-2"></view>
							<view>记住密码</view>
						</view>
						<view>忘记密码?</view>
					</view>
					<view class="btn-group">
						<button  class="btn-group-1">登陆</button>
					</view>
					<view class="visitor-btn">先去逛逛</view>
				</view>
				<view class="login-right">
					<view class="login-right-box">
						<view class="head-img"/>
						<view class="right-text">
							<view class="text">注</view>
							<view class="text">册</view>
							<view class="text">新</view>
							<view class="text">用</view>
							<view class="text">户</view>
						</view>
					</view>
				</view>
			</view>
		</view>
		<view class="bottom-box" v-if="0">
			<view class="bottom-box-1">
				<img src="/static/image-13.png" class="bottom-box-2"/>
				<view  class="bottom-box-3">
					<view class="bottom-box-4">全站App客户端</view>
					<view class="bottom-box-5">点击下载</view>
				</view>
			</view>
			<view class="bottom-box-1">
				<img src="/static/image-13.png" class="bottom-box-2"/>
				<view  class="bottom-box-3">
					<view class="bottom-box-4">全站App客户端</view>
					<view class="bottom-box-5">点击下载</view>
				</view>
			</view>
		</view>
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

		}
	}
</script>

<style lang="less" scoped>
	.bottom-box{
		align-items: center;
		justify-content: space-between;
		display: flex;
		.bottom-box-1{
			background: rgba(0, 0, 0, .55);
			border-radius: 4px;
			width: 48%;
			height: 1rem;
			justify-content: center;
			display: flex;
			color: #fff;
			align-items: center;
		}
		.bottom-box-2{
			width: 0.6rem;
			height: 0.6rem;
			border-radius: 0.08rem;
			margin-right: 0.16rem;
		}
		.bottom-box-3{
			text-align: left;
		}
		.bottom-box-4{
			font-size: 0.2rem;
			height: 0.5rem;
			display: block;
			line-height: 0.6rem;
		}
		.bottom-box-5{
			color: #4b65de;
			font-size: 0.26rem;
			line-height: 1.4;
		}
	}
	.btn-group{
		width: 100%;
		text-align: center;
		.btn-group-1{
			width: 100%;
			height: 0.9rem;
			line-height: 0.9rem;
			border: none;
			border-radius: 0.45rem;
			font-size: 0.28rem;
			color: #ffffff;
			opacity: 0.5;
			background-color: #4b65de;
		}
		.btn-active{
			opacity: 1;
			background: #4b65de;
		}
	}
	.visitor-btn{
		margin-top: 0.3rem;
		text-align: center;
		color: #fff;
	}
	.content{
		width: 100vw;
		height: 100vh;
		background: url(/static/image-1.jpg) no-repeat left center;
		background-attachment: fixed;
		background-size: cover;
		.top-box{
			width: 100%;
			padding: 1rem .42rem .9rem;
			-webkit-box-sizing: border-box;
			box-sizing: border-box;
			position: relative;
			.top-logo{
				width: 3.04rem;
				height: 1.2rem;
				margin: 0 auto .32rem;
				background: url(/static/image-2.png) no-repeat center center;
				background-size: contain;
			}
			.top-title{
				width: 5.16rem;
				display: flex;
				flex-flow: row nowrap;
				margin: 0 auto 0.2rem;
				justify-content: center;
				align-items: center;
				.line{
					flex: 1;
					height: 1px;
					background: rgba(255, 255, 255, .5);
				}
				.title{
					flex: 0 0 1.6rem;
					text-align: center;
					font-size: 0.23rem;
					color: #ffffff;
				}
			}
			.bottom-logo{
				display: flex;
				justify-content: space-between;
				flex-flow: row nowrap;
				font-size: 0.24rem;
				.left{
					padding-left: 5em;
				}
				.logo{
					height: 1.36rem;
				}
				.right{
					padding-right: 5em;
				}
			}
		}
		.login-box{
			margin: 0px auto;
			.login-inner{
				align-items: stretch;
				width: 7.02rem;
				height: 7rem;
				border: none;
				margin: 0 auto;
				padding-bottom: 0.2rem;
				justify-content: center;
				display: flex;
				flex-flow: row nowrap;
				.login-left{
					border-radius: 0.2rem 0 0 0.2rem;
					background-color: rgba(216, 216, 216, .3);
					flex: 1;
					padding: 0 0.4rem 0.4rem;
					box-sizing: border-box;
					font-size: 0.24rem;
					.top-login{
						height: 1.5rem;
						line-height: .5rem;
						padding: .4rem 0.2rem 0;
						text-align: center;
						font-size: 0.36rem;
						color: #ffffff;
					}
					.input-box{
						margin-bottom: 0.18rem;
						.input{
							display: flex;
							flex-flow: row nowrap;
							justify-content: flex-start;
							align-items: center;
							width: 5.2rem;
							height: 0.9rem;
							padding: 0 0.3rem;
							margin-bottom: 0.2rem;
							border-radius: 0.45rem;
							box-sizing: border-box;
							background-color: rgba(0, 0, 0, .5);
							font-size: 0.24rem;
							.input-left{
								background: url(/static/image-6.png) no-repeat center center;
								background-size: contain;
								flex: 0 0 0.4rem;
								width: 0.4rem;
								height: 0.4rem;
								margin-right: 0.2rem;
							}
							.input-left2{
								background: url(/static/image-7.png) no-repeat center center;
								background-size: contain;
							}
							.input-middle{
								flex: 1;
								.input-1{
									display: block;
									width: 100%;
									margin-top: 0.04rem;
									font-size: 0.24rem;
									color: #ffffff;
									padding-left: 0;
									text-align: justify;
								}
							}
							.input-right{
								background: url(/static/image-10.png) no-repeat center center;
								background-size: contain;
								width: 0.32rem;
								height: 0.32rem;
							}
							.input-right2{
								background: url(/static/image-8.png) no-repeat center center;
								background-size: contain;
							}
							.input-right3{
								background: url(/static/image-10.png) no-repeat center center;
								background-size: contain;
								width: 0.32rem;
								height: 0.32rem;
								margin-right: .08rem;
							}
						}
					}
				}
				.login-right{
					position: relative;
					flex: 0 0 1rem;
					border-radius: 0 0.2rem 0.2rem 0;
					background-color: rgba(0, 0, 0, .4);
					.login-right-box{
						position: absolute;
						width: 100%;
						top: 50%;
						left: 50%;
						transform: translate(-50%, -50%);
						.head-img{
							width: 0.56rem;
							height: 0.56rem;
							margin: 0 auto 0.23rem;
							background: url(/static/image-5.png) no-repeat center center;
							background-size: contain;
						}
						.right-text{
							text-align: center;
							.text{
								display: block;
								margin-bottom: 0.1rem;
								font-size: 0.28rem;
								color: #ffffff;
							}
						}
					}
				}
			}
		}
	}
	.other-opera{
		display: flex;
		flex-flow: row nowrap;
		justify-content: space-between;
		align-items: center;
		width: 100%;
		padding: 0 0.3rem;
		margin-bottom: .4rem;
		box-sizing: border-box;
		font-size: 0.2rem;
		color: #ffffff;
		.other-opera-1{
			display: flex;
			align-items: center;
		}
		.other-opera-2{
			display: inline-block;
			width: 0.32rem;
			height: 0.32rem;
			margin-right: 0.09rem;
			background: url(/static/image-11.png) no-repeat center center;
			background-size: contain;
		}
	}
</style>
