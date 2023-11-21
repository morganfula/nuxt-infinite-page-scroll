<template>
	<div class="main-page">
		<HeroSection />

		<TheSection
			:title="content.section1.title"
			:description="content.section1.description" />

		<TheSection
			:title="content.section2.title"
			:description="content.section2.description"
			isBlack />

		<TheSection
			:title="content.section3.title"
			:description="content.section3.description" />

		<TheFooter />

		<div class="wrapper-for-infinity-scroll">
			<HeroSection />
		</div>
	</div>
</template>

<script setup>
	const content = {
		section1: {
			title: 'Nulla  odio',
			description:
				'Pellentesque posuere risus sit amet turpis sodales fermentum. Mauris nisl purus, suscipit eu lacus at, tristique consequat urna. Nam sit amet diam at dui pretium ornare. Curabitur nec pulvinar elit, tempor consequat magna. Cras iaculis cursus sollicitudin. Mauris tristique sed eros eu hendrerit. Proin eu vulputate tellus, sed commodo libero. Praesent suscipit leo sed urna fringilla fringilla. Vivamus ultrices vestibulum odio in auctor.',
		},
		section2: {
			title: ' sollicitudin ',
			description:
				'Cras sollicitudin sapien quis quam ultricies, ac aliquam ante tempor. Praesent congue varius dolor, vel pulvinar libero consequat ac. Quisque rutrum in libero in sollicitudin. Sed sit amet dignissim diam. Quisque condimentum scelerisque lorem, at fringilla risus pulvinar ac. Aliquam imperdiet eros condimentum ex aliquet posuere. Etiam interdum id lorem ut interdum. Quisque non ultrices ipsum. Vivamus justo ex, consectetur sit amet orci vel, volutpat efficitur velit. Duis faucibus, orci at tempor pharetra, lorem nibh varius justo, efficitur commodo erat magna non est. ',
		},
		section3: {
			title: 'Duis  malesuada',
			description:
				'Suspendisse aliquet ante non nibh pharetra, in pharetra mi efficitur. In et mauris justo. Nam eleifend pretium dictum. Proin maximus ipsum at nulla consectetur semper. Aenean pharetra ac dui vel facilisis. Suspendisse sed malesuada diam.',
		},
	};
</script>

<style lang="scss" scoped>
	.wrapper-for-infinity-scroll {
		height: 100svh;
		overflow: hidden;
	}
</style>
