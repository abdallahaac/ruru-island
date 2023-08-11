<template>
	<!-- mobile view -->
	<div
		class="mobile lg:hidden flex flex-col items-center justify-center w-full text-center"
	>
		<div
			class="card relative bg-red-300 h-full w-screen"
			style="margin-top: 60px"
		>
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img1.jpg"
				alt=""
				srcset=""
				class="w-full h-full object-cover"
			/>
			<div
				class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400"
					>_</span
				>
			</div>
		</div>
		<div class="card relative bg-red-300 h-full w-screen">
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img2.jpg"
				alt=""
				srcset=""
				class="w-full h-full object-cover"
			/>
			<div
				class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400"
					>_</span
				>
			</div>
		</div>

		<div class="card relative bg-red-300 h-full w-screen">
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img3.jpg"
				alt=""
				srcset=""
				class="w-full h-full object-cover"
			/>
			<div
				class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400"
					>_</span
				>
			</div>
		</div>
		<div class="card relative bg-red-300 h-full w-screen">
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img4.jpg"
				alt=""
				srcset=""
				class="w-full h-full object-cover"
			/>
			<div
				class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400"
					>_</span
				>
			</div>
		</div>
		<div class="card relative bg-red-300 h-full w-screen">
			<img
				src="https://haar.qodeinteractive.com/wp-content/uploads/2018/02/home6-img5.jpg"
				alt=""
				srcset=""
				class="w-full h-full object-cover"
			/>
			<div
				class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
			>
				<span class="text-white text-5xl font-semibold">Lorem</span>
				<span class="text-white text-6xl font-semibold blinking text-red-400"
					>_</span
				>
			</div>
		</div>

		<!-- Other card divs -->
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@media (max-width: 1024px) {
	.mobile {
		display: flex;
		justify-content: center; /* Center horizontally */
		align-items: center; /* Center vertically */
	}
	.card-c {
		background-color: rgb(37, 37, 37);
	}

	.card {
		width: 100%;
		position: relative;
	}

	.overlay {
		transition: opacity 0.3s;
	}

	img {
		object-fit: cover;
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
}
</style>
