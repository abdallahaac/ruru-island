<template class="">
	<!-- desktop view -->
	<div class="desktop">
		<div
			class="flex flex-col lg:flex-row w-screen h-screen justify-center items-center"
		>
			<div class="relative flex w-full lg:w-1/2 lg:h-full overflow-hidden">
				<img
					src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img1.jpg"
					alt=""
					srcset=""
					class="cards inset-0 w-full h-full object-cover transition duration-300 lg:h-screen"
				/>
				<div
					class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
				>
					<span class="text-white text-5xl font-semibold">Lorem</span>
					<span class="text-white text-6xl font-semibold blinking text-red-400"
						>_</span
					>
				</div>
			</div>
			<div class="grid lg:grid-cols-2 h-full gap-0">
				<!-- First Image -->
				<div
					class="flex bg-red-500 relative h-full overflow-hidden lg:h-screen"
				>
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img2-550x550.jpg"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
							>_</span
						>
					</div>
				</div>
				<!-- Second Image -->
				<div class="flex bg-red-500 relative h-full overflow-hidden">
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img3-550x550.jpg"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
							>_</span
						>
					</div>
				</div>
				<!-- Third Image -->
				<div class="flex bg-red-500 relative h-full overflow-hidden">
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img4-550x550.jpg"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
							>_</span
						>
					</div>
				</div>
				<!-- Fourth Image -->
				<div class="flex bg-red-500 relative h-full overflow-hidden">
					<img
						src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img5-550x550.jpg"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<div
						class="absolute inset-0 bg-zinc-800 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Lorem</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
							>_</span
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
@media (max-width: 1024px) {
	.cards {
		display: inline-block;
		width: 100%;
		height: 100%;
		max-width: 90%; /* Adjust this value to control the maximum width of the images */
		margin: 0 auto; /* Center the images horizontally */
		object-fit: contain;
	}
	.desktop {
		display: none;
	}
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
