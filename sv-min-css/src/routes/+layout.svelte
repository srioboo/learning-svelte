<script lang="ts">
	import './styles.css'; // o importar pico desde los estilos
	import Header from './Header.svelte';
</script>

<div>
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>
</div>

<style>
	/**
		Estilos del layout
	*/
</style>
