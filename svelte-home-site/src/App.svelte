<script lang="ts">
	import MainCard from "./components/MainCard.svelte";
	import Card from "./components/Card.svelte";
	
</script>

<main>


	<MainCard/>


	
	{#each ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10'] as numbers}
		<div style="margin: 20%;">
		<Card><h1 style="text-align: center;">{numbers}</h1></Card>	
		</div>
	{/each}
	
</main>

<style>
	
	main {
		margin: 0;
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	

	h1 {
		color: #777777;
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