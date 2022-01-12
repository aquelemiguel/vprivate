<script lang="ts">
	import * as json from '../public/db.json';
	import Service from "../components/Service.svelte";
	const data = json['default'];
</script>

<main>
	{#each data as service, i}
		<Service data={service} altTheme={i % 2 !== 0}/>
	{/each}
</main>