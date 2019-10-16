<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	header {
		position: fixed;
		top: 0;
		left: 0;
		right: 0;
		text-align: center;
		nax-height: 4em;
		border-bottom: 1px solid rgba(255,62,0,0.1);
	}

	main {
		position: fixed;
		top: 4em;
		left: 0;
		right: 0;
		bottom: 3em;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
		max-height: 90vh;
		overflow-y: scroll;
	}

	footer {
		position: fixed;
		bottom: 0;
		left: 0;
		right: 0;
		text-align: center;
		height: 3em;
	}
</style>

<header>
	<Nav {segment}/>
</header>

<main>
	<slot></slot>
</main>

<footer>
	<p>
		&copy; 2000-2019 Estalio Consulting Inc.
	<p>
</footer>
