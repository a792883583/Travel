<template>
	<div>
  	<home-header></home-header>
  	<home-swiper></home-swiper>
  	<home-icons></home-icons>
  	<home-reacommend></home-reacommend>
  	<home-weekend></home-weekend>
  </div>
</template>
<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
import HomeReacommend from './components/Recommend'
import HomeWeekend from './components/Weekend'


export default{
  name: 'home',
  components:{
  	HomeHeader,
  	HomeSwiper,
  	HomeIcons,
  	HomeReacommend,
  	HomeWeekend
  }
}
</script>
<style>
  
</style>