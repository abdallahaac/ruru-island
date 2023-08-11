<script setup lang="ts">
const route = useRoute();
const { data } = await useAsyncData(`content-${route.path}`, () =>
	queryContent().where({ _path: route.path }).findOne()
);
</script>

<template>
	<div class="text-black">
		<Header />
	</div>
	<main>
		<header class="bg-white flex items-align justify-center">
			<div class="content-container">
				<div class="content">
					<img
						class="banner-image shadow-sm"
						:src="data.body.children[0].children[0].props.src"
						alt=""
					/>

					<div class="content-info bg-red-300">
						<h1>{{ data.title }}</h1>
						<p>{{ data.body.children[2].children[0].value }}</p>
					</div>
				</div>
			</div>
		</header>
	</main>
</template>

<style scoped>
/* Styles for the image */
.banner-image {
	width: 100%; /* Make the image fill the entire width */
	max-height: 500px; /* Adjust the height as needed */
	object-fit: cover; /* Maintain aspect ratio and cover container */
	margin-top: 100px;
}

/* Styles for the content container */
.content-container {
	display: flex;
	flex-direction: column;
	align-items: center;
	text-align: center;
}

/* Styles for the content */
.content {
	margin-top: 20px;
}

/* Styles for the heading */
.content h1 {
	font-size: 24px;
	color: #333;
}

/* Styles for the paragraph */
.content p {
	font-size: 16px;
	line-height: 1.5;
}

.nav :deep(div) {
	color: black;
	display: flex;
	justify-content: space-between;
}
.nav {
	position: fixed;
	z-index: 1;
}

main {
	height: 200vh;
}
</style>
