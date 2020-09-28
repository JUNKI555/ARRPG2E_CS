<script lang="ts">
	import Title from './components/Title.svelte';
	import ProfileInfo from './components/ProfileInfo.svelte';
	import LifePath from './components/LifePath.svelte';
	import ClassInfo from './components/ClassInfo.svelte';
	export let name: string;
	name = "hoge";
</script>

<main>
<Title version={"0.01"} />
<hr style="margin-bottom: 2em;">

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">基本情報</p>
		<div class="ar-nes-container-inner">
			<ProfileInfo/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">ライフパス</p>
		<div class="ar-nes-container-inner">
			<LifePath/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">キャラクターLv1時のクラス</p>
		<div class="ar-nes-container-inner">

		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">所属ギルド</p>
		<div class="ar-nes-container-inner">

		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">ゲッシュ</p>
		<div class="ar-nes-container-inner">

		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">クラス情報</p>
		<div class="ar-nes-container-inner">
			<ClassInfo/>
		</div>
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

	.ar-nes-container-outer {
		text-align: left;
		max-width: 100%;
		margin-top: 1em;

		@media screen and (max-width: 480px) {
			max-width: 100%;
		}
	}

	.ar-nes-container-inner {
		margin: 0 -1em;

		&.hide {
			visibility: hidden;
			height: 0;
		}
	}
</style>
