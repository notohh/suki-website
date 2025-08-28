<script lang="ts">
	import { page } from '$app/state'
	import Dead from '$lib/assets/suki_down.png'
</script>

<svelte:head>
	<title>{page.status}: {page.error?.message}</title>
</svelte:head>

<div
	class="bg-base flex h-screen flex-col items-center justify-center font-display"
>
	<img class="mb-4" src={Dead} alt="" />
	<h1 class="text-4xl font-bold">{page.status}: {page.error?.message}</h1>
</div>
