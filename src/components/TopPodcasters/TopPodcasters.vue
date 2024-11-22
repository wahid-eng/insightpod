<script setup>
import Podcaster from '../Podcaster/Podcaster.vue';
</script>

<template>
	<section>
		<div class="container py-16">
			<h2
				class="text-5xl font-extrabold text-orange-950 text-center w-96 mx-auto"
			>
				Top Podcasters of the Week
			</h2>
			<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mt-8">
				<Podcaster
					name="Mr. Mark Smith"
					streams="1.6 million streams"
					photo="/src/assets/images/top-podcaster-1.webp"
					background="bg-yellow-300"
				/>
				<Podcaster
					name="Nadia Lestary"
					streams="2 million streams"
					photo="/src/assets/images/top-podcaster-2.webp"
				/>
				<Podcaster
					name="Evan Castera"
					streams="5 million streams"
					photo="/src/assets/images/top-podcaster-3.webp"
					background="bg-pink-300"
				/>
				<Podcaster
					name="Stefy Catlyna"
					streams="1 million streams"
					photo="/src/assets/images/top-podcaster-4.webp"
					background="bg-green-300"
				/>
			</div>
		</div>
	</section>
</template>
