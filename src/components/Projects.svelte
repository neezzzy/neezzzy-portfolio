<script lang="ts">
	import type { Project } from '../types/project';
	export let projects: Project[];

	import ProjectCard from '../components/ProjectCard.svelte';
</script>

<section id="projects" class="">
	<hr class="border-t border-gray-300 my-4" />
	<div class="project-wrapper">
		<h2 class="lg:text-5xl max-md:text-3xl font-bold leading-5 text-uppercase letter-spacing-minus-1 tracking-tighter">
			Projects
		</h2>
		<div class="project-text lg:text-2xl max-md:text-xl mt-4">
			<p class="leading-8">
				I continue to add new projects to my portfolio. Here are some of the latest projects that I
				have worked on.
			</p>
		</div>
		<div class="w-fit mx-auto grid grid-cols-1 lg:grid-cols-3 md:grid-cols-2 justify-items-center justify-center gap-y-20 gap-x-14 mt-10 mb-5">
			{#each projects as project}
				<ProjectCard {project} />
			{/each}
		</div>
	</div>
</section>

<style>
	.project-wrapper {
		position: relative;
		align-items: flex-start;
		margin-inline: auto;
		padding-top: 2rem;
		padding-bottom: 2rem;
		gap: 2rem;
		width: 100%;
		max-width: 60rem;
	}

	.project-text {

	}
</style>
