<script setup>
import Button from '../Button/Button.vue';
</script>

<template>
	<section class="bg-orange-50 py-16">
		<div
			class="container flex flex-col-reverse md:flex-row gap-y-12 items-center"
		>
			<div class="flex-1">
				<h1
					class="font-extrabold leading-tight text-orange-950 text-5xl lg:text-6xl xl:text-7xl 2xl:text-8xl"
				>
					Navigating Ideas, Sharing Insights.
				</h1>
				<p class="xl:text-xl my-4 lg:my-8">
					Unlock invaluable wisdom personalized for you in our top-notch
					podcast. Dive into episodes designed to deliver relevant insights that
					cater to your interests and needs.
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
			<div class="flex-1">
				<img
					src="../../assets/images/hero-thumbnail.webp"
					alt="Hero thumbnail"
					class="max-w-xs lg:max-w-md xl:max-w-lg 2xl:max-w-xl mx-auto md:ms-auto md:me-0"
					loading="lazy"
				/>
			</div>
		</div>
	</section>
</template>
