<script setup>
import Button from '../Button/Button.vue';
import thumbnail from '../../assets/images/listen.webp';
</script>

<template>
	<section>
		<div class="container py-16">
			<div
				class="bg-orange-950 py-16 px-8 text-white rounded-3xl grid grid-cols-1 lg:grid-cols-2 items-center gap-16"
			>
				<div>
					<img
						:src="thumbnail"
						alt="Difference Thumbnail"
						loading="lazy"
						class="lg:max-w-md xl:max-w-lg 2xl:max-w-xl mx-auto"
					/>
				</div>
				<div>
					<h2 class="text-3xl lg:text-5xl font-extrabold lg:leading-tight">
						Listen to the latest and exciting podcast content
					</h2>
					<p class="my-8">
						Don't miss the valuable updates in each session and listen existing
						podcast
					</p>
					<Button
						class="bg-yellow-300 border-yellow-300 justify-between ps-6 pe-2 py-1.5 min-w-52"
						>Listen Now
						<svg
							width="48"
							height="48"
							viewBox="0 0 48 48"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M24 44C35.0457 44 44 35.0457 44 24C44 12.9543 35.0457 4 24 4C12.9543 4 4 12.9543 4 24C4 35.0457 12.9543 44 24 44Z"
								fill="white"
							/>
							<path
								d="M18.1992 23.999V21.039C18.1992 17.219 20.8992 15.679 24.1992 17.579L26.7592 19.059L29.3192 20.539C32.6192 22.439 32.6192 25.559 29.3192 27.459L26.7592 28.939L24.1992 30.419C20.8992 32.319 18.1992 30.759 18.1992 26.959V23.999Z"
								fill="#532822"
							/>
						</svg>
					</Button>
				</div>
			</div>
		</div>
	</section>
</template>
