<script>
	import ServerLogo from './components/ServerLogo.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<div class="logotext">	
		<p> Serveri24h </p>
	</div>
	<div class="placeholder"></div>
	<ServerLogo></ServerLogo>
</section>

<style>

@font-face {
	font-family: "myFont";
	src: url("$lib/fonts/TrueType/SFFedora.ttf");
}

@font-face {
	font-family: "voluteFont";
	src: url("$lib/fonts/volute/Volute.ttf");
}
@font-face {
	font-family: "voluteFont";
	src: url("$lib/fonts/stonestory/StoneStoryEBO.ttf");
}


section {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items: center;
		flex: 1;
		height: 100%;
	}

	.logotext {
		display: flex;
		position: absolute;
		top: 2em;
		flex-direction: column;
		align-items: center;
		padding: 0em;
		width: 100%;
	}

	.logotext p {
		font-family: "myFont";
		font-size: 4.5em;
		font-weight: 100;
		color: var(--color-theme-1);
		font-weight: 900;
	}

	.placeholder {
		height: 6em;
	}

	
</style>
