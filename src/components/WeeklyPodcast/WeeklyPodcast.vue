<script setup>
import Button from '../Button/Button.vue';
import Podcast from '../Podcast/Podcast.vue';
import podThumb1 from '../../assets/images/weekly-pod-1-thumb.webp';
import podThumb2 from '../../assets/images/weekly-pod-2-thumb.webp';
import podThumb3 from '../../assets/images/weekly-pod-3-thumb.webp';
</script>

<template>
	<section>
		<div class="container py-16">
			<div class="flex items-center gap-x-8 justify-between">
				<h2 class="text-3xl lg:text-5xl font-extrabold text-orange-950">
					Weelky Podcast
				</h2>
				<Button class="text-yellow-300 border-yellow-300 min-w-36"
					>See All</Button
				>
			</div>
			<div class="grid grid-weekly-podcast gap-8 mt-8">
				<Podcast
					id="1"
					:thumbnail="podThumb1"
					title="Quarter-life crisis"
					author="Brock Leslar"
					time="23:30"
					background="bg-green-300"
				/>
				<Podcast
					id="1"
					:thumbnail="podThumb2"
					title="Finance Gen Z"
					author="Allen John"
					time="45:00"
					background="bg-yellow-300"
				/>
				<Podcast
					id="1"
					:thumbnail="podThumb3"
					title="Love, Family, dan"
					author="Aidan &amp; Friends"
					time="16:20"
					background="bg-pink-300"
				/>
				<Podcast
					id="1"
					:thumbnail="podThumb1"
					title="Freedom of life"
					author="Brock Leslar"
					time="18:33"
					background="bg-orange-950"
				/>
			</div>
		</div>
	</section>
</template>

<style scoped>
.grid-weekly-podcast {
	grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
}
</style>
