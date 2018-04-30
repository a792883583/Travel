<template>
	<div class="wrapper">
		<swiper :options="swiperOption">
			<swiper-slide v-for="item of swiperlist" :key="item.id">
				<img class="swiper-img" :src="item.imgUrl" />
			</swiper-slide>
			<div class="swiper-pagination" slot="pagination"></div>
		</swiper>
	</div>
</template>

<script>
	export default {
		name: 'HomeSwiper',
		data() {
			return {
				swiperOption: {
					pagination:'.swiper-pagination',
					loop:true
				},
				swiperlist:[{
					id:'0001',
					imgUrl:'http://img1.qunarzz.com/piao/fusion/1804/c4/1cdd28811593b802.jpg_640x200_0d7b87b6.jpg'
				},{
					id:'0002',
					imgUrl:'http://img1.qunarzz.com/piao/fusion/1804/fa/1932440360b42e02.jpg_640x200_07b74613.jpg'
				}]
			}
		}
	}
</script>

<style lang="stylus" scoped>
	.wrapper >>> .swiper-pagination-bullet-active
		background:#fff
	.wrapper
		overflow: hidden
		width:100%
		height:0
		padding-bottom: 31.25%
		background:#eee
		.swiper-img
			width:100%
</style>