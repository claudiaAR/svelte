
<script>
	let count = 0;

	// `$:` betyder kör igen när dessa värden ändras
	$: dubbel = count * 2;
	$: fyrdubbel = dubbel * 2;

	function handleClick() {
		count += 1;
	}
</script>

<main>
	<button on:click={handleClick}>
		Click me
	</button>

	<h1>
		Clicked {count} {count === 1 ? 'time' : 'times'}
	</h1>

	<p>{count} * 2 = {dubbel}</p>
	<p>{dubbel} * 2 = {fyrdubbel}</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	h1 {
		color: #18a4e0;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	p {
		background: #222d6d;
		color: #f8b4c1;
		font-size: 2rem;
	}
	button{
		background: #222d6d;
		color: #f8b4c1;
		border: none;
		padding: 2rem;
		font-size: 1.5rem; 
		text-transform: uppercase;
	}
</style>










