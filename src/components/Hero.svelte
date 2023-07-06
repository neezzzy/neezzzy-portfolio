<script lang="ts">
	export let linkedInUrl: string;
	export let githubUrl: string;
	import { Heading, Button } from 'flowbite-svelte';
</script>

<header>
	<section class="h-screen">
		<div class="flex flex-col h-full justify-center items-center ">
			<Heading class="hero-title text-center py-4 px-6 hero">
				<span class="title-wrapper">
					<span class="title">
						<div>Russell</div>
						<div>Nizamov</div>
						<div>Web</div>
						<div>Developer</div>
					</span></span
				></Heading
			>
			<div class="flex justify-center md:justify-between gap-4 p-5">
				<Button outline class="">
					<a aria-label="Visit Ruslan Nizamov's LinkedIn" target="_blank" href={linkedInUrl}
						>LinkedIn</a
					>
				</Button>
				<Button outline class="">
					<a aria-label="Visit Ruslan Nizamov's GitHub" target="_blank" href={githubUrl}>GitHub</a
					></Button
				>
			</div>
		</div>
	</section>
</header>

