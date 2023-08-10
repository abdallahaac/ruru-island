<template>
	<Header />

	<div class="flex w-full w-screen">
		<div class="flex flex-col w-full">
			<div class="h-[588px] w-[200%] bg-red-300"></div>
			<div class="h-full w-full bg-red-300"></div>
		</div>

		<div class="flex flex-wrap w-screen w-full h-[100vh]">
			<div class="min-h-fit min-w-[420px] max-w-full bg-red-500"></div>
			<div class="min-h-fit min-w-[420px] max-w-full bg-red-400"></div>
			<div class="min-h-fit min-w-[420px] max-w-full bg-red-600"></div>
			<div class="min-h-fit min-w-[420px] max-w-full bg-red-400"></div>
		</div>
	</div>
</template>

<script setup></script>

<style lang="scss" scoped>
.max-w-full {
	width: 100%;
}
</style>
