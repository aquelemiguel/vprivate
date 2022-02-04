<script>
	import page from 'page';
	import Home from './Home.svelte';
	import Services from './Services.svelte';
	import Partners from './Partners.svelte';
	import About from './About.svelte';

	let current = Home;

	page('/', () => (current = Home));
	page('/services', () => (current = Services));
	page('/partners', () => current = Partners);
	page('/about', () => current = About);
	page.start();
</script>

<main>
	<svelte:component this={current} />
</main>