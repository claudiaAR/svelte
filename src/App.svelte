
<script>
	let count = 0;

	$: dubbel = count * 2;
	$: fyrdubbel = count * 2;

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
		max-width: 15rem;
		margin: 0 auto;
		/* background:#f3e5e3; */
		box-shadow: 15px 23px 29px -6px rgba(34,45,109,0.45);
	}
	h1 {
		color: #18a4e0;
		text-transform: uppercase;
		font-size: 3.8em;
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










