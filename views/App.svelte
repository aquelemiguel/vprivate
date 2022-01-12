<script>
	import page from 'page';
	import Home from './Home.svelte';
	import Services from './Services.svelte';

	let current = Home;

	page('/', () => (current = Home));
	page('/services', () => (current = Services));
	page.start();
</script>

<main>
	<svelte:component this={current} />
</main>