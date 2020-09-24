<script lang="ts">
	import Title from './components/Title.svelte';
	//export let name: string;
</script>

<main>
<Title version={"0.01"} />



<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style lang="scss">
	main {
		text-align: center;
		padding: 1em;
		width: 1024px;
		margin: 0 auto;
	}

	@media (max-width: 480px) {
		main {
			width: 480px;
		}
	}
</style>
