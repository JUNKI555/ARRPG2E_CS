<script lang="ts">
	import Title from './components/Title.svelte';
	import CharacterName from './components/CharacterName.svelte';
	import ProfileInfo from './components/ProfileInfo.svelte';
	import LifePath from './components/LifePath.svelte';
	import ClassInfoLv1 from './components/ClassInfoLv1.svelte';
	import Guild from './components/Guild.svelte';
	import Geis from './components/Geis.svelte';
	import ClassInfo from './components/ClassInfo.svelte';
	export let name: string;
	name = "hoge";

	let hideProfileInfo = false
	,hideLifePath = true
	,hideClassInfoLv1 = true
	,hideGuild = true
	,hideGeis = true
	,hideClassInfo = false;

</script>

<main>
<Title version={"0.01"} />
<hr style="margin-bottom: 2em;">

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title">
			<i class="nes-icon is-small heart"></i>キャラクター名&nbsp;
		</p>
		<div class="ar-nes-container-inner">
			<CharacterName/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideProfileInfo = !hideProfileInfo}">
			<i class="nes-icon is-small heart"></i>基本情報&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideProfileInfo}">
			<ProfileInfo/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideLifePath = !hideLifePath}">
			<i class="nes-icon is-small heart"></i>ライフパス&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideLifePath}">
			<LifePath/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideClassInfoLv1 = !hideClassInfoLv1}">
			<i class="nes-icon is-small heart"></i>キャラクターLv1時のクラス&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideClassInfoLv1}">
			<ClassInfoLv1/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideGuild = !hideGuild}">
			<i class="nes-icon is-small heart"></i>所属ギルド&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideGuild}">
			<Guild/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideGeis = !hideGeis}">
			<i class="nes-icon is-small heart"></i>ゲッシュ&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideGeis}">
			<Geis/>
		</div>
	</div>
</div>

<div class="ar-nes-container-outer">
	<div class="nes-container is-rounded is-dark with-title">
		<p class="title" on:click="{() => hideClassInfo = !hideClassInfo}">
			<i class="nes-icon is-small heart"></i>クラス情報&nbsp;<i class="nes-icon close is-small"></i>
		</p>
		<div class="ar-nes-container-inner" class:hide="{hideClassInfo}">
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
