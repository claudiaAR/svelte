
<script>
	let count = 0;

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
</main>

<style>
	body{
		padding: 6rem;
	}
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

	button{
		background: #222d6d;
		color: #f8b4c1;
		border: none;
		padding: 2rem;
		font-size: 1.5rem; 
		text-transform: uppercase;
	}


</style>