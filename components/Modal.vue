<template>
	<transition name="modal-fade" mode="out-in">
		<div
			v-if="isOpen"
			class="fixed top-0 left-0 w-full h-full flex-col justify-center items-center bg-black bg-opacity-50"
			@click="closeModal"
		>
			<div class="bg-white p-5 shadow-lg w-full h-full flex flex-col">
				<div class="flex justify-end w-full">
					<Icon
						@click="closeModal"
						name="radix-icons:eye-closed"
						size="40"
						id="icon"
						class="flex"
					/>
				</div>
				<div class="">test</div>

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
#icon {
	color: #cf2e2e;
	margin-right: 26px;
	padding: 5px;
	cursor: pointer;
	display: flex;
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
