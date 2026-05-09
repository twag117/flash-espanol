<script>
	import favicon from '$lib/assets/favicon.svg'
	import '@drop-in/graffiti'

	let { children } = $props()
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header class="header">
	<h6>Flash Español</h6>
</header>


<main>
	{@render children()}
</main>

<footer>
	© 2026 TechForge 365. All Rights Reserved.
</footer>

<style>
	header, main, footer {
		padding: var(--vs-base);
	}
</style>