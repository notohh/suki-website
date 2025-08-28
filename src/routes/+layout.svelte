<script lang="ts">
	import favicon from '$lib/assets/favicon.png'
	import Navbar from '$lib/components/Navbar.svelte'
	import Footer from '$lib/components/Footer.svelte'
	import '../app.css'

	let { children } = $props()
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="flex min-h-screen flex-col">
	<Navbar />
	<main class="grow">
		{@render children?.()}
	</main>
	<Footer />
</div>
