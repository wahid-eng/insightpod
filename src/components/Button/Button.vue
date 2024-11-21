<script setup>
import { defineProps, defineEmits } from 'vue';
const props = defineProps({
	type: {
		type: String,
		default: 'button',
	},
	disabled: {
		type: Boolean,
		default: false,
	},
});

const emit = defineEmits(['click']);
const handleClick = (event) => {
	if (!props.disabled) {
		emit('click', event);
	}
};
</script>

<template>
	<button
		:class="[
			'border inline-flex items-center rounded-full p-4 min-w-52 font-bold text-orange-950 border-orange-950',
			disabled ? 'opacity-50 cursor-not-allowed' : '',
		]"
		:disabled="disabled"
		@click="handleClick"
	>
		<slot>Button</slot>
	</button>
</template>
