<script lang="ts">
	import * as json from '../public/db.json';
	import Service from "../components/Service.svelte";
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';

	const data = json['default'];
</script>

<Header />
<main>
	{#each data as service, i}
		<Service data={service} />
	{/each}
</main>
<Footer />