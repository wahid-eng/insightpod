<script setup>
import Podcaster from '../Podcaster/Podcaster.vue';
import podcaster1 from '../../assets/images/top-podcaster-1.webp';
import podcaster2 from '../../assets/images/top-podcaster-2.webp';
import podcaster3 from '../../assets/images/top-podcaster-3.webp';
import podcaster4 from '../../assets/images/top-podcaster-4.webp';
</script>

<template>
	<section>
		<div class="container py-16">
			<h2
				class="text-3xl lg:text-5xl font-extrabold text-orange-950 text-center lg:w-96 lg:mx-auto leading-tight"
			>
				Top Podcasters of the Week
			</h2>
			<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 mt-8">
				<Podcaster
					name="Mr. Mark Smith"
					streams="1.6 million streams"
					:photo="podcaster1"
					background="bg-yellow-300"
				/>
				<Podcaster
					name="Nadia Lestary"
					streams="2 million streams"
					:photo="podcaster2"
				/>
				<Podcaster
					name="Evan Castera"
					streams="5 million streams"
					:photo="podcaster3"
					background="bg-pink-300"
				/>
				<Podcaster
					name="Stefy Catlyna"
					streams="1 million streams"
					:photo="podcaster4"
					background="bg-green-300"
				/>
			</div>
		</div>
	</section>
</template>
