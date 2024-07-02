<template>
	<section>
		<div id="view-more">
			<p>MOVIE</p>
			<p>VIEW MORE</p>
		</div>
		<swiper :modules="modules" :slidesPerView="1" :spaceBetween="50" :loop="true" :autoplay="{ delay: 3000 }">
			<swiper-slide><img src="../assets/movie01.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie02.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie03.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie04.jpg" /></swiper-slide>
			<swiper-slide><img src="../assets/movie05.jpg" /></swiper-slide>
		</swiper>
		<!-- <div id="color"></div> -->
	</section>
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
section {
	padding-top: 70px;
	padding-bottom: 47vw;
	width: 100%;
	height: 650px;
	background: linear-gradient(180deg, transparent 80%, white 80%);
	backdrop-filter: blur(5px);
}
#view-more {
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
	align-items: flex-start;
	p {
		margin: 0 0 25px;
		padding: 0 5%;
		font-family: aktiv-grotesk, sans-serif;
		font-weight: 400;
		font-style: normal;
		color: #fff;
		font-size: 16px;
		letter-spacing: 0.3em;
	}
	p:nth-child(2) {
		font-size: 11px;
	}
}
.swiper {
	width: 125%;
	height: 450px;
	position: relative;
	top: 10%;
	left: 50%;
	transform: translateX(-50%);
}

.swiper-slide img {
	width: 100%;
	height: 100%;
	object-fit: contain;
}
</style>
