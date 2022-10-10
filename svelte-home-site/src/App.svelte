<script lang="ts">
	let name = "Awesomesauce";
	let numClick = 0;
	let showText = false;
	let event = ()=>{
		numClick++
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	
	<button on:mouseenter={event}>You've clicked the button {numClick} time(s)!</button>
	{#if showText}
		<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	{/if}

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