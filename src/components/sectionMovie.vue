<template>
	<div id="view-more">
		<p>MOVIE</p>
		<p>VIEW MORE</p>
	</div>
	<div class="container">
		<swiper :modules="modules" :slidesPerView="3" :spaceBetween="50" :loop="true" :autoplay="{ delay: 3000 }">
			<swiper-slide><img src="../assets/movie01.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie02.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie03.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie04.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie05.jpg" /></swiper-slide>
		</swiper>
	</div>
	<div id="color"></div>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css/bundle";

// import required modules
import { Autoplay } from "swiper/modules";

export default {
	components: {
		Swiper,
		SwiperSlide
	},
	setup() {
		return {
			modules: [Autoplay]
		};
	}
};
</script>

<style scoped lang="scss">
#view-more {
	width: 60%;
	height: 30vh;
	letter-spacing: 0.3rem;
	text-align: center;
	p:nth-child(1) {
		font-size: 22px;
		font-weight: 400;
		color: white;
		margin-bottom: 40px;
		padding-top: 10%;
	}
	p:nth-child(2) {
		font-size: 12px;
		font-weight: 400;
		color: white;
	}
}

.container {
	position: relative;
	overflow: hidden;
	width: 100%;
	height: 50%;
}

.swiper {
	width: 125%;
	position: absolute;
	left: 50%;
	transform: translateX(-50%);
}

.swiper-slide {
	text-align: center;
	/* Center slide text vertically */
	display: flex;
	justify-content: center;
	align-items: center;
}

.swiper-slide img {
	display: block;
	width: 100%;
	height: 100%;
	object-fit: contain;
}
#color {
	width: 100%;
	height: 10vh;
	background: #fff;
}
</style>
