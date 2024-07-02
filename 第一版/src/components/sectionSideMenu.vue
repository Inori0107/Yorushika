<template>
	<header>
		<a href="#"><img src="../assets/xs_logo.jpg" /></a>
		<div>
			<span
				>ME <br />
				NU</span
			>
		</div>
	</header>
</template>

<script setup></script>

<style scoped>
header {
	position: relative;
	z-index: 1000;
	background: #fff;
	width: 100%;
	height: 60px;
	img {
		margin-left: 45px;
	}
	div {
		background: #acd0d1;
		position: absolute;
		top: 0;
		right: 0;
		width: 60px;
		height: 60px;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		span {
			display: block;
			height: 100%;
			width: 100%;
			padding: 11px 0px 8px 18px;
			color: #fff;
			letter-spacing: 0.6rem;
			font-size: 12px;
			line-height: 1.5;
		}
	}
}
</style>
