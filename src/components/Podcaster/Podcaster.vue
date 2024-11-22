<script setup>
defineProps({
	id: Number,
	name: String,
	streams: String,
	photo: String,
	background: {
		type: String,
		default: 'bg-orange-950',
	},
});
</script>

<template>
	<div
		:class="[
			'px-8 pt-8 rounded-3xl flex flex-col justify-between overflow-hidden',
			background,
		]"
	>
		<h4 class="text-white mb-6 font-bold text-4xl">
			{{ name }}
		</h4>
		<div>
			<p
				class="px-4 py-2 mb-6 rounded-full bg-white text-black inline-flex text-sm xl:text-lg"
			>
				{{ streams }}
			</p>
		</div>
		<img :src="photo" :alt="`${name} Photo`" loading="lazy" />
	</div>
</template>
