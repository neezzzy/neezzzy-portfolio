<script lang="ts">
	import { Button } from 'flowbite-svelte';
	export let icon: string;
	export let href: string;
</script>

<Button
	class="m-2 !p-2 dark:bg-slate-900"
	color="dark"
	{href}
	aria-label="Visit Ruslan Nizamov's LinkedIn"
	role="button"
	target="_blank"
>
	<img src={icon} class="social-icon" alt="Visit Ruslan Nizamov's linkedin" />
</Button>
