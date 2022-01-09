<script lang="ts">
import Footer from "../components/Footer.svelte";
import Service from "../components/Service.svelte";

</script>

<main>
	<Service />
	<Footer />
</main>

<style>
	main {
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>