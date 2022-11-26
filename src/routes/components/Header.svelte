<script>
	import { page } from '$app/stores';
</script>

<header>
	<nav>
		<svg viewBox="0 0 250 100">
			<circle cx="100" cy="50" r="50"/>
			<rect x="100" y="-50" width="150" height="200" fill="red"/>
			{#each [0,1,2,3] as ix}
				{#each [0,1,2] as iy}
					<rect x="{110+ix*25}" y="{15+iy*25}" width="20" height="12" class="server-button"/>
				{/each}
			{/each}
		</svg>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">Whoami</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/contact') ? 'page' : undefined}>
				<a href="/contact">Contact</a>
			</li>
		</ul>
		<svg viewBox="0 0 250 100">
			<rect x="0" y="-50" width="150" height="200" fill="red"/>
			<circle cx="150" cy="50" r="50"/>
			<circle cx="50" cy="50" r="25" class="server-circle"/>
			<circle cx="120" cy="50" r="25" class="server-circle"/>
		</svg>
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

        --backbone-color: #d0d0d0;
    }

	svg circle {
		fill: var(--background);
	}

	svg rect {
		fill: var(--background);
	}

	.server-circle {
		stroke: #330000;
		stroke-width: 4px;
	}

	@keyframes animate_boxes {

		0% {
			fill: var(--box-color1);
		}

		50% {
			fill: var(--box-color1);
		}

		75% {
			fill: #6f2abe;
		}

		100% {
			fill: var(--box-color1);
		}
	}

	.server-button {
		transition: transform 2s;
		fill: box-color1;
		animation-name: animate_boxes;
		animation-duration: 5s;
		animation-iteration-count: infinite;
	}

	header {
		display: flex;
		justify-content: space-around;
		height: 4em;
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

	svg {
		height: 3em;
		display: block;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: #330000;
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}
</style>
