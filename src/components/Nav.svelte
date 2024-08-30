<script>
	export let segment;
</script>

<style>
	nav {
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	.logo {
		margin-top: -0.5em;
	}

	.selected {
		position: relative;
		display: inline-block;
	}

	.selected::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}
</style>

<nav>
	<ul>
		<li><a href='.'><img class='logo' alt='Estalio' src='logo.png'></a></li>
		<li><a class='{segment === undefined ? "selected" : ""}' href='.'>About Us</a></li>
		<li><a class='{segment === "faq" ? "selected" : ""}' href='faq'>FAQ</a></li>
		<li><a class='{segment === "contact" ? "selected" : ""}' href='contact'>Contact</a></li>

	</ul>
</nav>
