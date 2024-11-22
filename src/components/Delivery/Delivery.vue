<script setup>
import thumbnail from '../../assets/images/delivery.webp';
</script>

<template>
	<section>
		<div class="container py-16">
			<div
				class="flex flex-col-reverse lg:flex-row gap-x-16 gap-y-8 justify-between items-center"
			>
				<h2 class="flex-1 text-4xl lg:text-5xl font-extrabold text-orange-950">
					<span class="leading-tight"
						>Our podcast dives into diverse topics like life, finances,
					</span>
					<span class="opacity-40 leading-tight"
						>and personal experiences, offering valuable insights and practical
						advice.</span
					>
				</h2>
				<div class="lg:w-1/3">
					<img
						:src="thumbnail"
						alt="Deliver Photo"
						loading="lazy"
						class="w-7/12 mx-auto"
					/>
				</div>
			</div>
			<div
				class="flex flex-col lg:flex-row gap-x-16 gap-y-8 justify-between items-center mt-16"
			>
				<div class="flex flex-1 justify-between gap-x-8 w-full">
					<div class="flex flex-col">
						<span class="text-orange-500 text-6xl font-extrabold">5+</span>
						<span>Awards Gained</span>
					</div>
					<div class="flex flex-col">
						<span class="text-orange-500 text-6xl font-extrabold">12+</span>
						<span>Years of Experience</span>
					</div>
					<div class="flex flex-col">
						<span class="text-orange-500 text-6xl font-extrabold">230+</span>
						<span>Podcasters</span>
					</div>
				</div>
				<p class="lg:w-1/3">
					Unlock invaluable wisdom personalized for you in our top-notch
					podcast. Dive into episodes designed to deliver relevant insights that
					cater to your interests and needs.
				</p>
			</div>
		</div>
	</section>
</template>
