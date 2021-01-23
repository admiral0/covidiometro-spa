<script>
	import About from "./routes/About.svelte";
	import Dashboard from "./routes/Dashboard.svelte";

	import Router from 'svelte-spa-router'

	const routes = {
		'/': Dashboard,
		'/about': About,

		'*': Dashboard,
	}

</script>

<nav>
	<a href="#/">Dashboard</a>
	<a href="#/about">About</a>
</nav>

<Router {routes} />

<style>
	nav {
		border-bottom: 1px solid black;
		padding-bottom: 3px;
	}
	nav a {
		font-size: large;
		padding: 5px;
	}

	nav a:hover {
		font-weight: bold;
	}
</style>
