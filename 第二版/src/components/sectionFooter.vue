<template>
	<section>
		<div class="bnr" data-aos="fade-right" data-aos-offset="300" data-aos-easing="ease-in-sine" data-aos-duration="1000">
			<!-- <div class="bnr"> -->
			<ul>
				<li>
					<a href="https://sp.yorushika.com/?lang=zh-tw&_ga=2.190609899.1176093959.1719389554-1625497109.1719120652"><img src="../assets/bnr01.png" /></a>
				</li>
				<li>
					<a href="https://store.plusmember.jp/yorushika/"><img src="../assets/bnr02.jpeg" /></a>
				</li>
				<li>
					<a href="https://store.plusmember.jp/yorushika/"><img src="../assets/bnr03.png" /></a>
				</li>
				<li id="copyright">
					© YORUSHIKA 版權所有。<br />
					許可證號：9012207290Y38029
				</li>
			</ul>
		</div>
	</section>
</template>

<script setup>
import AOS from "aos";
import "aos/dist/aos.css";
import DataView from "primevue/dataview";

AOS.init({
	once: true
});
</script>

<style scoped lang="scss">
section {
	margin-left: 60px;
	width: calc(100% - 60px);
	height: 35vh;
	background: transparent;
	backdrop-filter: blur(5px);
	img {
		height: 65px;
	}
}

.bnr {
	padding-top: 100px;
	ul {
		display: flex;
		li {
			list-style-type: none;
			margin-right: 15px;
		}
	}
}
#copyright {
	margin-left: auto;
	margin-right: 30px;
	text-align: center;
	font-size: 12px;
	color: #fff;
	line-height: 2.5;
}
</style>
