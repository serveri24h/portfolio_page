<script>
    import HeaderTemplate from "./HeaderTemplate.svelte";

	let data = [
		{
			url: '/',
			name: 'Home',
			children: null,
		},
		{
			url: '/about',
			name: 'WhoAmI',
			children: [
				{
					url: '/education',
					name: 'Education',
					children: null,
				},
				{
					url: '/skills',
					name: 'Skills',
					children: null,

				}
			],
		},
		{
			url: '/contact',
			name: 'Contact',
			children: null,
		},
	]

</script>

<header>
	<nav>
		<HeaderTemplate nav_data={data} />
	</nav>
	<placeholder-box>
		<div></div>
	</placeholder-box>
</header>

<style>

	:root {
        --box-color1: #101010;
        --box-color2: #a40000;
        --box-color3: #2f6900;
    }


	header {
		display: flex;
		justify-content: space-around;
		height: 6.5em;
	}

	placeholder-box {
		height: 100%;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: var(--backbone-color);
		position: fixed;
		width: 100%;
	}
</style>
