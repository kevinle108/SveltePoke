<script>
	let level = 5
</script>
<main>
	<button class="center" on:click={() => level++}>Level: {level}</button>
	{#if level >= 16 && level < 36}
		<img class="center" src="https://img.pokemondb.net/sprites/black-white/anim/normal/charmeleon.gif" alt="">
		{:else if level >= 36}
			<img class="center" src="https://img.pokemondb.net/sprites/black-white/anim/normal/charizard.gif" alt="">
		{:else}
		<img class="center" src="https://img.pokemondb.net/sprites/black-white/anim/normal/charmander.gif" alt="">
	{/if}
	
</main>

<style>
	main {
		display: block;
		margin: 0 auto;
	}
	.center {
		display: block;
		margin: 0 auto;
		width: 10%;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>