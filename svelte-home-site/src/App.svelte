<script lang="ts">
	import MainCard from "./components/MainCard.svelte";
	let name = "Awesomesauce";
	let numClick = 0;
	let showText = false;
	let event = ()=>{
		numClick++
	};
</script>

<main>
	<MainCard/>

	{#each ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10'] as numbers}
		<h1>{numbers}</h1>
	{/each}
</main>

<style>
	main {
		
		text-align: center;
		padding: 1em;
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