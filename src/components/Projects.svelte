<script lang="ts">
	import type { Project } from '../types/project';
	export let projects: Project[];
	import { Heading, P } from 'flowbite-svelte';
	import ProjectCard from '../components/ProjectCard.svelte';
</script>

<section id="projects" class="p-4">
	<hr class="border-t border-gray-300 my-4" />
	<div class="flex flex-col">
		<div class="text-center">
			<Heading
				tag="h2"
				class="mb-4 mt-4 text-4xl font-extrabold dark:text-indigo-700 text-indigo-600"
				>Projects</Heading
			>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				I continue to add new projects to my portfolio. Here are some of the latest projects that I
				have worked on. In the past few months, I have had the opportunity to work on a diverse
				range of projects, showcasing my versatility and adaptability.
			</P>
			<P class="mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
				These projects have allowed me to refine my skills in design, development, and project
				management, while also providing valuable hands-on experience in collaborating with diverse
				teams and meeting client expectations.
			</P>
			<div
				class="w-fit mx-auto grid grid-cols-1 lg:grid-cols-3 md:grid-cols-2 justify-items-center justify-center gap-y-20 gap-x-14 mt-10 mb-5"
			>
				{#each projects as project}
					<ProjectCard {project} />
				{/each}
			</div>
		</div>
	</div>
</section>

<style>
</style>
