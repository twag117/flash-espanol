<script>
	import favicon from '$lib/assets/favicon.svg'
	import '@drop-in/graffiti'

	let { children } = $props()
</script>

<svelte:head>
	<!-- <link rel="icon" href={favicon} /> -->
	<!-- <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text x=%2250%25%22 y=%2250%25%22 dominant-baseline=%22middle%22 text-anchor=%22middle%22 font-size=%2290%22 fill=%22white%22>Ñ</text></svg>"> -->
	<link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22 fill=%22white%22>Ñ</text></svg>">

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