<template>
	<!-- component <sidebar> -->
	<sectionSideMenu></sectionSideMenu>

	<section id="bg_pic">
		<img :src="bg_picture" />
	</section>

	<section id="section-carousel">
		<!-- component <Carousel> -->
		<sectionCarousel></sectionCarousel>
	</section>

	<section id="section-news">
		<!-- component <News> -->
		<sectionNews></sectionNews>
	</section>

	<section id="section-movie">
		<!-- component <Movie> -->
		<sectionMovie></sectionMovie>
	</section>

	<footer>
		<!-- component <Footer> -->
		<sectionFooter></sectionFooter>
	</footer>
	<ScrollTop />
</template>

<script setup>
import sectionSideMenu from "./components/sectionSideMenu.vue";
import sectionCarousel from "./components/sectionCarousel.vue";
import sectionNews from "./components/sectionNews.vue";
import sectionFooter from "./components/sectionFooter.vue";
import sectionMovie from "./components/sectionMovie.vue";

import logo from "./assets/logo.png";
import bg_picture from "./assets/bg_picture.jpeg";
import "./style/main.scss";

import AOS from "aos";
import "aos/dist/aos.css";
AOS.init({
	once: true
});
</script>

<style scoped lang="scss">
aside {
	background: rgb(172, 208, 209);
	position: fixed;
	top: 0;
	left: 0;
	width: 60px;
	height: 100vh;
	transition: all 0.3s 0s ease;
	// z-index: 100;
}
#section-carousel {
	width: 100%;
	height: 40vh;
	background: #fff;
	padding: 0px 30px 30px 90px;
}
#section-news {
	width: 100%;
	height: 50vh;
	background: #fff;
	padding: 0px 30px 30px 90px;
	display: flex;
	justify-content: center;
}
#section-movie {
	margin-left: 60px;
	width: calc(100% - 60px);
	height: 80vh;
	background: linear-gradient(90deg, transparent 60%, white 60%);
	backdrop-filter: blur(5px);
}
footer {
	margin-left: 60px;
	width: calc(100% - 60px);
	height: 35vh;
	background: transparent;
	backdrop-filter: blur(5px);
}

:deep(.p-scrolltop-icon) {
	color: aqua;
}
</style>
