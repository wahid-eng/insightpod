<script setup>
const props = defineProps({
	id: Number,
	thumbnail: String,
	title: String,
	author: String,
	time: String,
});
</script>

<template>
	<div class="bg-slate-100 flex gap-4 rounded-3xl p-4">
		<img
			:src="thumbnail"
			:alt="`${title} thumbnail`"
			class="bg-orange-950 rounded-[1.75rem] w-28 h-28 object-contain"
			loading="lazy"
		/>
		<div class="flex flex-col relative flex-1">
			<h4 class="font-medium text-orange-950 text-xl">{{ title }}</h4>
			<p class="text-base mt-2">{{ author }}</p>
			<p class="font-extrabold text-orange-950 mt-auto">{{ time }}</p>
			<Button class="p-0 border-none absolute right-0 bottom-0">
				<svg
					width="48"
					height="48"
					viewBox="0 0 48 48"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						d="M24 44C35.0457 44 44 35.0457 44 24C44 12.9543 35.0457 4 24 4C12.9543 4 4 12.9543 4 24C4 35.0457 12.9543 44 24 44Z"
						class="fill-yellow-300"
					/>
					<path
						d="M18.1992 23.999V21.039C18.1992 17.219 20.8992 15.679 24.1992 17.579L26.7592 19.059L29.3192 20.539C32.6192 22.439 32.6192 25.559 29.3192 27.459L26.7592 28.939L24.1992 30.419C20.8992 32.319 18.1992 30.759 18.1992 26.959V23.999Z"
						class="fill-orange-950"
					/>
				</svg>
			</Button>
		</div>
	</div>
</template>
