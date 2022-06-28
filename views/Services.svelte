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
		<div class="service-container">
			<Service data={service} />
		</div>
	{/each}
</main>
<Footer />

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 8rem 0 4rem 0;
		background-color: whitesmoke;
	}

	.service-container {
		width: 70%;
		height: 70%;
	}

	.service-container:not(:last-of-type) {
		margin-bottom: 2rem;
	}
</style>