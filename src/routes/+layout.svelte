<script>
	import '../app.css';
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';

	let { children } = $props();

</script>

<div class="flex min-h-screen flex-col bg-background text-foreground">
	<Header />
	{@render children?.()}
	<Footer />
</div>

