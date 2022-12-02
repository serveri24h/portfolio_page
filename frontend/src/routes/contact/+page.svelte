<script>
	import GitLogo from '../components/GitLogo.svelte';
</script>

<div class="text-column">
	<div class="info-container">
		<h1> Contact me </h1>
		<p>severi.vapalahti@gmail.com </p>
	</div>

	<div class="info-container">
		<p> Find me from </p>
		<div>
			<a href="https://github.com/serveri24h">
				<GitLogo></GitLogo>
			</a>
		</div>
	</div>
</div>

<style>
	.info-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.info-container p, h1 {
		display: flex;
        width: 100%;
		justify-content: center;
        object-fit: contain;
    }

	.info-container div {
		display: flex;
		flex-direction: row;
		justify-content: center;
        align-items: center;
	}

	.info-container a {
		display: block;
        justify-content: center;
        width: 10em;
        height: 100%;
    }
</style>