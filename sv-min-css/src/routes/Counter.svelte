<script lang="ts">
	import { spring } from 'svelte/motion';

	let count = 0;

	const displayed_count = spring();
	$: displayed_count.set(count);
	$: offset = modulo($displayed_count, 1);

	function modulo(n: number, m: number) {
		// handle negative numbers
		return ((n % m) + m) % m;
	}
</script>

<div class="grid">
	<button on:click={() => (count -= 1)} aria-label="Decrease the counter by one">
	<strong>-</strong>
	</button>

	<div>
		<div style="transform: translate(0, {100 * offset}%)">
			<strong class="hidden" aria-hidden="true">{Math.floor($displayed_count + 1)}</strong>
			<strong>{Math.floor($displayed_count)}</strong>
		</div>
	</div>

	<button on:click={() => (count += 1)} aria-label="Increase the counter by one">
	<strong>+</strong>
	</button>
</div>

<style>
	/*
	Estilos
	*/
	.hidden {
		visibility: hidden;
	}
</style>
