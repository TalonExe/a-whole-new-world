<script>
	import '../app.css';
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';

	let { children } = $props();

</script>

<svelte:head>
	<link
        href="https://cdn.jsdelivr.net/npm/prismjs@1.29.0/themes/prism-solarizedlight.min.css"
        rel="stylesheet"
    />
</svelte:head>

<div class="flex min-h-screen flex-col bg-background text-foreground">
	<Header />
	{@render children?.()}
	<Footer />
</div>

