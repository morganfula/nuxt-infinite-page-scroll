<template>
	<div id="viewport">
		<slot />
	</div>
</template>

<script setup>
	import { useSmoothScroll } from '~/composables/useSmoothScroll';

	onMounted(() => {
		useSmoothScroll();
	});
</script>

<style lang="scss"></style>
