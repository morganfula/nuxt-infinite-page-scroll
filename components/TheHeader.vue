<template>
	<header class="header">
		<div class="header__head _container">
			<div class="header__logo">LOGO</div>

			<div class="header__link" v-for="link in links">
				{{ link }}
			</div>
		</div>
	</header>
</template>

<script setup>
	const links = ['about', 'contact'];
</script>

<style lang="scss" scoped>
	.header {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		z-index: $z-header;

		color: rgba($color-white, 0.8);
		text-transform: capitalize;
	}

	.header__head {
		display: flex;
		justify-content: space-between;
	}

	.header__logo {
		flex: 1 1 auto;
	}

	.header__link {
		margin-left: 16px;
	}
</style>
