<template class="">
	<!-- desktop view -->
	<div class="desktop">
		<div
			class="flex flex-col lg:flex-row w-screen h-screen justify-center items-center"
		>
			<div class="relative flex w-full lg:w-1/2 lg:h-full overflow-hidden">
				<img
					src="../assets/skull_dance.png"
					alt=""
					srcset=""
					class="cards inset-0 w-full h-full object-cover transition duration-300 lg:h-screen"
				/>
				<NuxtLink to="/posts/the-prisoner" class="card-link">
					<div
						class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
					>
						<span class="text-white text-5xl font-semibold">Ministrels</span>
						<span
							class="text-white text-6xl font-semibold blinking text-red-400"
							>_</span
						>
					</div>
				</NuxtLink>
			</div>
			<div class="grid lg:grid-cols-2 h-full gap-0">
				<!-- First Image -->
				<div
					class="flex bg-white z-1 relative h-full overflow-hidden lg:h-screen"
				>
					<img
						src="https://i.ibb.co/61F4QSX/bird.png"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<NuxtLink to="/posts/the-prisoner" class="card-link">
						<div
							class="card-c absolute inset-0 opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
						>
							<span class="text-white text-5xl font-semibold">Prisoner</span>
							<span
								class="text-white text-6xl font-semibold blinking text-red-400"
								>_</span
							>
						</div>
					</NuxtLink>
				</div>
				<!-- Second Image -->
				<div class="flex bg-red-500 relative h-full overflow-hidden">
					<img
						src="../assets/The_beast.png"
						alt=""
						srcset=""
						style="background-color: rgb(37, 37, 37)"
						class="cards inset-0 w-full h-full object-cover transition duration-300 object-contain"
					/>
					<NuxtLink to="/posts/the-moth" class="card-link">
						<div
							class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
						>
							<span class="text-white text-5xl font-semibold">Moth</span>
							<span
								class="text-white text-6xl font-semibold blinking text-red-400"
								>_</span
							>
						</div>
					</NuxtLink>
				</div>
				<!-- Third Image -->
				<div class="flex bg-white relative h-full overflow-hidden">
					<img
						src="../assets/the-wanderers.png"
						alt=""
						srcset=""
						style="background-color: rgb(37, 37, 37)"
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<NuxtLink to="/posts/the-prisoner" class="card-link">
						<div
							class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
						>
							<span class="text-white text-5xl font-semibold">Lorem</span>
							<span
								class="text-white text-6xl font-semibold blinking text-red-400"
								>_</span
							>
						</div>
					</NuxtLink>
				</div>

				<!-- Fourth Image -->
				<div class="flex bg-red-500 relative h-full overflow-hidden">
					<img
						src="../assets/tree.jpg"
						alt=""
						srcset=""
						class="cards inset-0 w-full h-full object-cover transition duration-300"
					/>
					<NuxtLink to="/posts/the-scribe" class="card-link">
						<div
							class="absolute inset-0 card-c opacity-0 transition duration-300 hover:opacity-100 flex items-center justify-center"
						>
							<span class="text-white text-5xl font-semibold">Scribe</span>
							<span
								class="text-white text-6xl font-semibold blinking text-red-400"
								>_</span
							>
						</div>
					</NuxtLink>
				</div>
			</div>
		</div>
	</div>
</template>

<script scoped></script>

<style lang="scss" scoped>
.h-full {
	height: 100%;
	width: 100%;
}
.blinking {
	animation: blink-animation 2s infinite;
	color: #f87171;
}
.card-c {
	background-color: rgb(37, 37, 37);
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
