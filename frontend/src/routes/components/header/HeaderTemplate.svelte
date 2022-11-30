<script>
	import { page } from '$app/stores';
    export let nav_data = [];
	export let root = '';
	console.log($page.url.pathname==='/');
</script>

<header_template>
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
        {#each nav_data as d }
        <li aria-current={  ($page.url.pathname.includes(d.url) && d.url!=='/') || (d.url==='/' && $page.url.pathname=='/') ? 'page' : undefined}>
            <a href="{root + d.url}">{d.name}</a>
            {#if d.children !== null }
            <div>
                <svelte:self nav_data={d.children} root={d.url}></svelte:self>
            </div>
            {/if}
        </li>
        {/each}
    </ul>
    <svg viewBox="0 0 250 100">
        <rect x="0" y="-50" width="150" height="200" fill="red"/>
        <circle cx="150" cy="50" r="50"/>
        <circle cx="50" cy="50" r="25" class="server-circle"/>
        <circle cx="120" cy="50" r="25" class="server-circle"/>
    </svg>
</header_template>

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

	header_template {
        display: flex;
        flex-direction: row;
        position: absolute;
		justify-content: space-around;
		height: 4em;
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

    li div {
        display: none;
        position: absolute;
        left: -168px;

    }

	li:hover div  {
		display: flex;
	}

	a {
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

	a:hover {
		color: var(--color-theme-1);
	}
</style>