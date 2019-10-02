<script>
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style>
	main {
		position: relative;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
		height: 100%;
	}

	footer {
		position: fixed;
		bottom: 0;
		left: 0;
		right: 0;
		text-align: center;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
	<footer>
		<p>
			&copy; 2000-2019 Estalio Consulting Inc.
		<p>
	</footer>
</main>
