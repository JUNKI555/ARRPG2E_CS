<script lang="ts">
	import Title from './components/Title.svelte';
	//export let name: string;
</script>

<main>
<Title version={"0.01"} />
<hr style="margin-bottom: 2em;">
<div class="ar-profile-info">
<div class="nes-container is-round is-dark with-title">
  <p class="title">基本情報</p>
  <p>Good morning. Thou hast had a good night's sleep, I hope.</p>
</div>
</div>

<hr style="margin-top: 2em;">
<footer class="creator-profile">
<span>Author:JUNKI555</span>
<span><a href="https://github.com/JUNKI555/ARRPG2E_CS" target="_blank" rel="noopener" aria-label="github"><i class="nes-icon github"></i></a> <a href="https://twitter.com/JUNKI555" target="_blank" rel="noopener" aria-label="twitter"><i class="nes-icon twitter"></i></a></span>
</footer>
</main>

<style lang="scss">
	main {
		text-align: center;
		padding: 2px;
		width: 100%;
		margin: 0 auto;
	}

	@media screen and (max-width: 480px) {
		main {
			width: 100%;
		}
	}

	.ar-profile-info {
		text-align: left;
		max-width: 50%;

		@media screen and (max-width: 480px) {
			max-width: 100%;
		}
	}
</style>
