<script>
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';

	export let segment;
</script>

<style>
	main {
		padding-top: 6rem;
		min-height: 100vh;
	}
</style>

<Nav {segment}/>

<main>
	<slot>
	</slot>
</main>

<Footer />

