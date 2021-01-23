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
	<a href="#/">Home</a>
	<a href="#/about">About</a>
</nav>

<Router {routes} />

<style>

</style>
