<template>
	<div
		class="lg:absolute sticky bg-white max-h-20 lg:h-20 flex flex-row text-align item-align justify-between w-full p-5 px-12 nav shadow-sm"
	>
		<div
			class="z-10 text-black inline-block cursor-pointer font-semibold tracking-widest lg:text-white text-lg"
		>
			<NuxtLink to="/">RURU ISLAND</NuxtLink>
		</div>
		<div
			class="z-10 inline-block cursor-pointer text-black lg:text-white burger"
		>
			<Icon name="radix-icons:hamburger-menu" size="28" />
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@media (max-width: 1024px) {
	.nav {
		position: fixed;
		z-index: 20;
	}
}
</style>
