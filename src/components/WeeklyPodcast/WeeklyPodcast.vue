<script setup>
import Button from '../Button/Button.vue';
import Podcast from '../Podcast/Podcast.vue';
</script>

<template>
	<section>
		<div class="container py-16">
			<div class="flex items-center gap-x-8 justify-between">
				<h2 class="text-5xl font-extrabold text-orange-950">Weelky Podcast</h2>
				<Button class="text-yellow-300 border-yellow-300 min-w-36"
					>See All</Button
				>
			</div>
			<div class="grid grid-weekly-podcast gap-8 mt-8">
				<Podcast
					id="1"
					thumbnail="/src/assets/images/weekly-pod-1-thumb.png"
					title="Quarter-life crisis"
					author="Brock Leslar"
					time="23:30"
				/>
				<Podcast
					id="1"
					thumbnail="/src/assets/images/weekly-pod-2-thumb.png"
					title="Finance Gen Z"
					author="Allen John"
					time="45:00"
				/>
				<Podcast
					id="1"
					thumbnail="/src/assets/images/weekly-pod-3-thumb.png"
					title="Love, Family, dan"
					author="Aidan &amp; Friends"
					time="16:20"
				/>
			</div>
		</div>
	</section>
</template>

<style scoped>
.grid-weekly-podcast {
	grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
}
</style>
