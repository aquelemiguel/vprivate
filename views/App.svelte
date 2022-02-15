<script>
	import page from 'page';
	import Home from './Home.svelte';
	import Services from './Services.svelte';
	import Partners from './Partners.svelte';
	import About from './About.svelte';
	import Contacts from './Contacts.svelte';
	import PrivacyPolicy from './PrivacyPolicy.svelte';

	let current = Home;

	page('/', () => (current = Home));
	page('/servicos', () => (current = Services));
	page('/parceiros', () => current = Partners);
	page('/sobre', () => current = About);
	page('/contactos', () => current = Contacts);
	page('/privacidade', () => current = PrivacyPolicy);
	page.start();
</script>

<main>
	<svelte:component this={current} />
</main>