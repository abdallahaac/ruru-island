<template>
	<transition name="modal-fade" mode="out-in">
		<div
			v-if="isOpen"
			class="fixed top-0 left-0 w-full h-full flex justify-center items-center bg-black bg-opacity-50"
			@click="closeModal"
		>
			<div class="bg-white p-5 rounded-lg shadow-lg w-full h-full">
				<div class="flex items-center justify-end">
					<p @click="closeModal">This is the modal content. Click to close.</p>
				</div>
				<div class="w-full h-full justify-center flex">hi</div>
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
