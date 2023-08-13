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
			class="z-20 inline-block cursor-pointer text-black lg:text-white burger"
			@click="toggleModal"
		>
			<Icon name="radix-icons:eye-open" size="37" id="eye-open" />
		</div>

		<!-- Modal component -->
		<Modal :isOpen="modalOpen" @close="closeModal" class="z-20" />
	</div>
</template>
<script>
import Modal from "@/components/Modal.vue"; // Adjust the path based on your project structure

export default {
	components: {
		Modal,
	},
	data() {
		return {
			modalOpen: false,
		};
	},
	methods: {
		toggleModal() {
			this.modalOpen = !this.modalOpen;
		},
		closeModal() {
			this.modalOpen = false;
		},
	},
};
</script>

<style lang="scss" scoped>
/* Add your existing styles */
@media (max-width: 1024px) {
	.nav {
		position: fixed;
		z-index: 20;
	}
	.eye-open {
		padding: 5px;
	}
}
</style>
