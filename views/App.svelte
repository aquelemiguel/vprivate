<script>
	import page from 'page';
	import Home from './Home.svelte';
	import Services from './Services.svelte';
	import About from './About.svelte';
	import Contacts from './Contacts.svelte';
	import PrivacyPolicy from './PrivacyPolicy.svelte';
	import Landing from './Landing.svelte';

	let current = Home;

	page('/', () => (current = Home));
	page('/servicos', () => (current = Services));
	page('/sobre', () => current = About);
	page('/contactos', () => current = Contacts);
	page('/privacidade', () => current = PrivacyPolicy);
	page('/landing', () => current = Landing);
	page.start();
</script>

<main>
	<svelte:component this={current} />
</main>