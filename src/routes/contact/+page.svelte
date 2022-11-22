<script>
    import github from '$lib/images/github.svg';
</script>

<div class="info-container">
	<p> Contact me </p>
	<p>email: kakko.pylly@homo.fi </p>
</div>

<div class="info-container">
	<p> Find me from </p>
	<div>
		<a href="https://github.com/sveltejs/kit">
			<img src={github} alt="GitHub" />
		</a>
	</div>
</div>

<style>
	.info-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.info-container img {
        width: 100%;
        height: 100%;
        object-fit: contain;
    }

	.info-container p {
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
        justify-content: center;
        width: 10em;
        height: 100%;
    }
</style>