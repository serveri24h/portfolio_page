<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import logo from '$lib/images/NewLogo1.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<div class="logotext">	
		<p> >>> Serveri24h >>> </p>
	</div>
	<p class="server-box">
		<span class="server">
			<picture>
				<source srcset={logo} type="image" />
				<img src={logo} alt="Welcome" />
			</picture>
		</span>
	</p>
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


	.server-box {
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 100%;
		padding: 0em;
	}

	.logotext {
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 0em;
		width: 100%;
	}

	.logotext p {
		font-family: "myFont";
		font-size: 3.5em;
		font-weight: 100;
		color: var(--color-theme-1);
		font-weight: 900;
	}



	.server {
		display: block;
		position: relative;
		width: 25%;
		height: 3em;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.server img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
	
</style>
