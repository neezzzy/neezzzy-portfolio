<script lang="ts">
	import type { Project } from '../types/project';
	export let project: Project;
</script>

<a href={project.link} class="w-72 bg-gray-100 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl">
	<img src={project.image} alt={project.title} class="h-80 w-72 object-cover rounded-t-xl" />
	<div class="px-4 py-3 w-72">
		<div class="flex items-center">
			<div class="flex flex-col justify-between px-4 py-6">
				<span class="block mb-4 text-2xl text-gray-900 leading-tight hover:text-blue-600">
					{project.title}
				</span>
				<p class="mb-4 text-gray-500">
					{project.description}
				</p>
			</div>
		</div>
	</div>
</a>

