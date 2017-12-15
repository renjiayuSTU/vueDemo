<template>
  <div>
  	<header class="header">
  		<div class="back">返回</div>
  		<div class="search"></div>
  		<div class="city">城市</div>
  	</header>
  	<swiper :options="swiperOption" ref="mySwiper">
	    <!-- slides -->
	    <swiper-slide>
	      <div class="swiper-img-con">
	      	<img class="swiper-img" src="../../img/1.jpg">
	      </div>
	    </swiper-slide>
	    <swiper-slide>
	      <div class="swiper-img-con">
	      	<img class="swiper-img" src="../../img/2.jpg">
	      </div>
	    </swiper-slide>
	    <!-- Optional controls -->
	    <div class="swiper-pagination"  slot="pagination"></div>
  	</swiper>
  </div>
</template>

<script>
export default {
  name: 'Index',
  data () {
    return {
	  swiperOption: {
	  	autoplay: 1000,
	 	direction: 'horizontal'
	  }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.header {
		display: flex;
	 	background: #05bad5;
	 	color: #fff;
	 	font-size: .12rem;
	}
	.back {
		width: .64rem;
		line-height: .86rem
	}
	.search {
		flex: 1;
		margin: .14rem .18rem;
		background: #fff;
		border-radius: .1rem;
	}
	.city {
		width: 1.14rem;
		line-height: .86rem;
		text-align: center;
	}
	.swiper-img-con {
		width: 100%
	}
	.swiper-img {
		width: 100%
	}
</style>
