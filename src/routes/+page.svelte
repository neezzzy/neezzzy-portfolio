<script>
	import Hero from '../components/Hero.svelte';
	import About from '../components/About.svelte';
	import Projects from '../components/Projects.svelte';
	import Footer from '../components/Footer.svelte';
	import CustomNav from '../components/CustomNav.svelte';
	import { projects } from '../data/project';

	const date = new Date().getFullYear();
</script>

<main class='bg-slate-100 dark:bg-gray-800'>
	<CustomNav />
	<Hero
		linkedInUrl="https://www.linkedin.com/in/nizamovruslan/"
		githubUrl="https://github.com/neezzzy"
	/>
	<About />
	<Projects {projects} />
	<Footer {date} />
</main>

<style>
	/* GLOBAL STYLES */
	:root {
		--primary-color: #030099;
		--black: #292929;
		--color-link: #a3a3ff;
		--surface-color: #292929;
		--card-title: #f96f68d8;
		--card-tech: #e3e3e3;
		--card-description: #c6c6c6d3;
		--text-color: #313131;
		--text-footer-color: #f5f5f5;
	}

	@font-face {
		font-family: 'Open Sans';
		font-style: normal;
		font-weight: 400;
		font-stretch: 100%;
		src: url(https://fonts.gstatic.com/s/opensans/v35/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4gaVI.woff2)
			format('woff2');
	}

	:global(h1, h2, h3) {
		font-family: 'Open Sans';
		text-transform: uppercase;
	}

	:global(h2) {
		color: var(--primary-color);
	}

	:global(p) {
		font-family: 'Ubuntu', sans-serif;
	}

	:global(ul) {
		padding: 0;
		list-style-type: none;
	}

	:global(a) {
		text-decoration: none;
	}

	:global(b) {
		color: var(--card-title);
	}

</style>
