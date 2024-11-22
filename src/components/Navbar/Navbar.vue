<script setup>
import Button from '../Button/Button.vue';
const props = defineProps({
	isNavbarVisible: Boolean,
});
const emit = defineEmits(['toggle-navbar']);
</script>

<template>
	<div
		:class="[
			'flex-1 fixed lg:static inset-0 bg-black/95 lg:bg-transparent text-white lg:text-inherit items-center lg:flex',
			isNavbarVisible ? 'flex' : 'hidden',
		]"
	>
		<Button
			class="absolute right-0 top-0 text-white border-none lg:hidden"
			@click="emit('toggle-navbar')"
			>Close</Button
		>
		<nav class="mx-auto text-2xl lg:text-lg">
			<ul class="flex items-center gap-y-8 flex-col lg:flex-row gap-4">
				<li><a href="#" class="px-4 py-2">About</a></li>
				<li><a href="#" class="px-4 py-2">Subscribe</a></li>
				<li><a href="#" class="px-4 py-2">Episode</a></li>
				<li><a href="#" class="px-4 py-2">Insiders</a></li>
			</ul>
		</nav>
	</div>
</template>
