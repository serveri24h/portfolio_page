<script>
    import github from '$lib/images/github.svg';
</script>

<footer>
	<div>	
		<div>	
			<div class="git-div">
				<img src={github} alt="SvelteKit" />
			</div>	
			<div class="text-div">
				<p>
					The source code for the page is in my
				</p>
				<p>
					<a href="https://github.com/serveri24h/portfolio_page">github</a>.
				</p>
			</div>	
			<div class="git-div"><img src={github} alt="SvelteKit" /></div>
		</div>
	</div>
</footer>

<style>

    footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 3.5em;
	}

	footer div {
		padding-bottom: 4em;
	}

	footer div div {
		display: flex;
		flex-direction: row;
		align-items: center;
		background-color: var(--backbone-color);
		padding-top: 0.5em;
		padding-bottom: 0.1em;
		padding-left: 1em;
		padding-right: 1em;
		border-radius: 5em;

	}

	.git-div {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		width: 3em;
		height: 50%;
	}

	.text-div {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	.text-div p {
		color: var(--basic-text-color-dark);
		line-height: 0.5;
	}

	img {
		object-fit: contain;
	}


	@media (min-width: 480px) {
		footer {
			padding: 5px;
		}
	}
</style>

