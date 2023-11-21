<template>
	<div class="hero">
		<TheHeader />
		<div class="hero__content _container">
			<div class="hero__title h1">lucky stones</div>
		</div>
	</div>
</template>

<script setup></script>

<style lang="scss" scoped>
	.hero {
		height: 150svh;
		background: url('/1.jpg');
		background-size: cover;
		background-position: center center;
		position: relative;
	}

	.hero__content {
		height: 100svh;
		display: flex;
		align-items: flex-end;
		color: $color-white;
		mix-blend-mode: overlay;
	}
</style>
