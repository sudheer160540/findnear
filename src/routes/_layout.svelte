<script>
	import Nav from '../components/UI/Nav.svelte';

	export let segment;
</script>

<style>
	main {
	position: relative;
    background-color: #f0f0f1;
    padding: 4em;
    margin: 0 auto;
    box-sizing: border-box;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>