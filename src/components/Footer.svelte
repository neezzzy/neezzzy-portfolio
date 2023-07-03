<script lang="ts">
	import { Heading, P } from 'flowbite-svelte';
	import SocialIcon from './SocialIcon.svelte';
	export let date: number;
</script>

<footer class="footer-section pt-5 mt-5 bg-gray-800 text-white dark:bg-gray-900" id="footer">
	<div class="text-center">
		<div class="flex flex-row justify-center mt-4">
			<!-- github -->
			<SocialIcon icon="icons/github.svg" href="https://github.com/neezzzy" />
			<SocialIcon icon="icons/email.svg" href="mailto:yottabitesapps@gmail.com" />
			<SocialIcon icon="icons/linkedin.svg" href="https://www.linkedin.com/in/nizamovruslan/" />
		</div>
		<!-- Copyright -->
		<P class="text-center lg:text-md max-md:text-sm p-1 text-white"
			>Made by Russell Nizamov © {date}</P
		>
	</div>
</footer>
