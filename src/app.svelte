<script>
	import Navigation from './layout/navigation.svelte';
	import Footer from './layout/footer.svelte';

	export let page;
</script>

<div id="app">
	<header>
		<Navigation />
	</header>

	<main>
		<svelte:component this={page.comp} {...page.props} />
	</main>


	<footer>
		<Footer />
	</footer>
</div>