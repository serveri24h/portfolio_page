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
	<p>
		Serveri24h is not a real company nor a brand. This is just a portfolio page.
	</p>
</section>

<style>

	@font-face {
		font-family: "myFont";
		src: url("$lib/fonts/TrueType/SFFedora.ttf");
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
		top: 1em;
		flex-direction: column;
		align-items: center;
		padding: 0em;
		width: 100%;
		background-color: aqua;
	}

	.logotext p {
		position: absolute;
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

