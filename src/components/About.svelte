<script>
	import Carousel from './Carousel.svelte';
	import { Heading, P } from 'flowbite-svelte';
</script>

<section id="about" class="px-4">
	<hr class="border-t border-gray-300" />
	<div class="flex flex-col">
		<div class="text-center">
			<Heading tag="h2" class="mb-4 mt-4 text-4xl font-extrabold dark:text-indigo-700 text-indigo-600">About me</Heading>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				Since I discovered programming six years ago, I have loved creating websites, making
				computer games, and coding solutions to solve real-world problems. I never thought that I
				might want to pursue it as a career in the future.
			</P>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				I graduated with a Master's Degree in Education. I've completed the Advanced Software
				Development certificate program.
			</P>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				In the past few years, I have learned and used React, JavaScript, Python, and Bootstrap to
				build the front-end. I also learned how to use Node, PHP, and Flask to implement the
				back-end.
			</P>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				I have over 50 different certificates of completion from <a
					aria-label="Visit LinkedIn Learning website"
					target="_blank"
					href="https://www.linkedin.com/learning/"><b>LinkedIn Learning</b></a
				>, <a aria-label="Visit Udemy" href="https://www.udemy.com/"><b>Udemy</b></a>, and
				<a target="_blank" aria-label="Visit Coursera" href="https://www.coursera.org/"
					><b>Coursera</b></a
				>, and I continually add new knowledge about new tech.
			</P>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400"
				>My current tech stack is below.</P
			>
		</div>
		<hr class="border-t border-gray-300 my-4" />

		<Carousel autoplay={2000} />
	</div>
</section>