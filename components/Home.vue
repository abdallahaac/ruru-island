<template>
	<div class="flex w-screen h-screen">
		<div class="relative flex w-1/2 h-full overflow-hidden">
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img1.jpg"
				alt=""
				srcset=""
				class="inset-0 w-full h-full object-cover z-0 transition duration-300"
			/>
			<div
				class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold text-bg">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400">
					_</span
				>
			</div>
		</div>
		<div class="flex w-full h-full">
			<div class="grid grid-cols-2 h-full">
				<!-- First Image -->
				<div
					class="flex bg-red-500 items-center justify-center text-align font-light tracking-widest text-2xl h-full relative"
				>
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img2-550x550.jpg"
						alt=""
						srcset=""
						class="inset-0 object-cover h-full z-0 transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
						>
							_</span
						>
					</div>
				</div>
				<!-- Second Image -->
				<div
					class="flex bg-red-500 items-center justify-center text-align font-light tracking-widest text-2xl h-full relative"
				>
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img3-550x550.jpg"
						alt=""
						srcset=""
						class="inset-0 object-cover h-full z-0 transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>

						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
						>
							_</span
						>
					</div>
				</div>
				<!-- Third Image -->
				<div
					class="flex bg-red-500 items-center justify-center text-align font-light tracking-widest text-2xl h-full relative"
				>
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img4-550x550.jpg"
						alt=""
						srcset=""
						class="inset-0 object-cover h-full z-0 transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
						>
							_</span
						>
					</div>
				</div>
				<!-- Fourth Image -->
				<div
					class="flex bg-red-500 items-center justify-center text-align font-light tracking-widest text-2xl h-full relative"
				>
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img5-550x550.jpg"
						alt=""
						srcset=""
						class="inset-0 object-cover h-full z-0 transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
						>
							_</span
						>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.h-full {
	height: 100%;
	width: 100%;
}
.blinking {
	animation: blink-animation 2s infinite;
	color: #f87171;
}

@keyframes blink-animation {
	0%,
	50%,
	100% {
		opacity: 1;
	}
	25%,
	75% {
		opacity: 0;
	}
}
</style>
