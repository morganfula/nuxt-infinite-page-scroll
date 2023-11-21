<template>
	<div class="section" :class="{ _black: isBlack }">
		<div class="section__content _container">
			<div class="section__title h2">
				{{ title }}
			</div>
			<div class="section__description p1">
				{{ description }}
			</div>
		</div>
	</div>
</template>

<script setup>
	defineProps({
		title: String,
		description: String,
		isBlack: Boolean,
	});
</script>

<style lang="scss" scoped>
	.section {
		height: 100svh;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.section__title {
		text-align: center;
	}

	.section__description {
		max-width: 1200px;
		margin: 0 auto;
		text-align: justify;
		text-align-last: justify;
		margin-top: 32px;
	}

	.section._black {
		background: $color-black;
		color: $color-white;
	}
</style>
