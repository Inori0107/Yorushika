<template>
	<section>
		<div id="news" data-aos="fade-up" data-aos-duration="2000">
			<h1>NEWS</h1>
			<p>VIEW MORE</p>
		</div>
		<div id="ad" data-aos="fade-up" data-aos-duration="2000">
			<ul>
				<li>
					<a href="https://yorushika.com/news/detail/11611?lang=zh-tw">
						<p class="date">2024.06.20 <span class="artists">suis</span></p>
						<p class="title">新潮文庫“文鳥・夢十夜/夏目漱石”的限定封面發售決定</p>
					</a>
				</li>
				<li>
					<a href="https://yorushika.com/news/detail/11610?lang=zh-tw">
						<p class="date">2024.06.14 <span class="artists">suis</span></p>
						<p class="title">suis的個人訪談刊登在《ROCKIN'ON JAPAN》8月號上</p>
					</a>
				</li>
				<li>
					<a href="https://yorushika.com/news/detail/11609?lang=zh-tw">
						<p class="date">2024.06.12 <span class="artists">YORUSHIKA</span></p>
						<p class="title">suis將作為嘉賓出演J-WAVE的《TOKIO HOT 100》</p>
					</a>
				</li>
			</ul>
		</div>
	</section>
</template>

<script setup>
import AOS from "aos";
import "aos/dist/aos.css";

AOS.init({
	once: true
});
</script>

<style scoped lang="scss">
section {
	display: flex;
	justify-content: center;
	align-items: center;
	height: 600px;
	background-color: #fff;
	padding: 80px 100px 130px 100px;
}
#news {
	width: 150px;
	height: 400px;
	padding-top: 30px;
	letter-spacing: 0.5rem;
	h1 {
		font-size: 22px;
		color: #000;
		margin-bottom: 20px;
	}
	p {
		font-size: 16px;
		font-weight: 200;
		color: #000;
	}
}
#ad {
	width: 800px;
	height: 400px;
	li {
		list-style-type: none;
		border-top: 1px solid #eaeaea;
		&:last-child {
			border-bottom: 1px solid #eaeaea;
		}
		a {
			padding: 24px 30px;
			cursor: pointer;
			display: flex;
			width: 100%;
			height: 100px;
			text-decoration: none;
			color: #000;
		}
	}
}
.date {
	font-size: 13px;
	font-weight: 400;
	color: #222;
	letter-spacing: 0.2rem;
	width: 250px;

	span {
		font-size: 10px;
		font-weight: 400;
		color: #fff;
		background: #acd0d1;
		padding: 3px 6px 3px 8px;
		margin-left: 10px;
	}
}
.title {
	margin-left: 5px;
}
</style>
