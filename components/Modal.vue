<template>
	<transition name="modal-fade" mode="out-in">
		<div
			v-if="isOpen"
			class="fixed top-0 left-0 w-full h-full flex-col justify-center items-center bg-black bg-opacity-50"
			@click="closeModal"
		>
			<div
				class="bg-white p-5 shadow-lg w-full h-full flex flex-col items-center"
			>
				<div class="flex justify-end w-full">
					<Icon
						@click="closeModal"
						name="radix-icons:eye-closed"
						size="40"
						id="icon"
						class="flex"
					/>
				</div>
				<div class="flex justify-center mt-[200px] flex-col uppercase links">
					<div class="flex link link-underline link-underline-black">
						<NuxtLink to="/"> Home </NuxtLink>
					</div>
					<div class="flex link link-underline link-underline-black">
						<NuxtLink to="/"> Home </NuxtLink>
					</div>
					<div class="flex link-underline link-underline-black">
						<NuxtLink to="/"> Home </NuxtLink>
					</div>
				</div>

				<!-- Additional modal content goes here -->
			</div>
		</div>
	</transition>
</template>

<script>
export default {
	props: {
		isOpen: Boolean,
	},
	methods: {
		closeModal() {
			this.$emit("close");
		},
	},
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap");
#icon {
	color: #cf2e2e;
	margin-right: 26px;
	padding: 5px;
	cursor: pointer;
	display: flex;
}

.links {
	color: #303030;
	font-size: 40px;
	font-family: "Poppins", sans-serif;
	font-weight: 700;
	margin-bottom: 20px;
}
.links > div {
	margin-bottom: 20px;
}
.links > div:hover {
	color: #f04c4b;
	transition: all 250ms;
}
.link-underline {
	border-bottom-width: 0;
	background-image: linear-gradient(transparent, transparent),
		linear-gradient(#fff, #fff);
	background-size: 0 5px;
	background-position: 0 100%;
	background-repeat: no-repeat;
	transition: background-size 0.5s ease-in-out;
}

.link-underline-black {
	background-image: linear-gradient(transparent, transparent),
		linear-gradient(#f04c4b, #f04c4b);
}

.link-underline:hover {
	background-size: 100% 5px;
	background-position: 0 100%;
}
/* Modal transition animation */
.modal-fade-enter-active,
.modal-fade-leave-active {
	transition: opacity 0.5s;
}
.modal-fade-enter,
.modal-fade-leave-to {
	opacity: 0;
}

/* Additional modal styling */
</style>
