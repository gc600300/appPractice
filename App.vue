<style lang="scss">
	/* 注意要写在第一行，同时给style标签加入lang="scss"属性 */
	@import "uview-ui/index.scss";
</style>
<script>
	export default {
		onLaunch: function() {
			            // tabbar中间按钮点击事件
			            uni.onTabBarMidButtonTap(function(e){
			                uni.navigateTo({
			                    url: "/pages/vip/index",
			                    animationType: "slide-in-bottom", // 动画类型
			                    animationDuration: 150, // 窗口动画持续时间，单位为 ms
			                    fail(err) {
			                        console.log(err)
			                    }
			                })
			            })
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	body {
		color: #666;
	}
	.select_area uni-checkbox .uni-checkbox-input {
		background-color: transparent !important
	}
	/*每个页面公共css */
	.vajraDistrict uni-swiper .uni-swiper-dot {
		width: 6px;
		height: 6px;
	}
	ul, li {
		list-style-type: none;
		padding: 0;
	}
</style>
