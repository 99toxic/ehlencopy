<script>
	// import HomeHeader from '$lib/HomeHeader.svelte';
	// import MainHeader from '$lib/MainHeader.svelte';
</script>

<slot />

<!-- {#if }
	<HomeHeader />
{:else}
	<MainHeader />
{/if} -->
<style>
	/* CSS RESET */
	:global(*),
	:global(*::before),
	:global(*::after) {
		box-sizing: inherit;
		margin: 0;
		padding: 0;
	}

	:global(html) {
		box-sizing: border-box;
		font-size: 62.5%; /* 10px / 16px = 62.5% -> 1rem = 10px */
	}

	/* Variables */
	:root {
		--color-black-2: #252a2c;
		--color-black: #000;
		--color-gradient-primary: linear-gradient(to right, #1b56e9 0%, #1aad92 100%);
		--color-primary: #1aad92;
		--color-secondary: #1b56e9;
		--color-tertiary: #f2f2f3;
		--color-transparent-black: rgba(0, 0, 0, 0.5);
		--color-transparent-white: rgba(255, 255, 255, 0.13);
		--color-white: #fff;

		--font-body: 'Raleway', sans-serif;
		--font-heading: 'Montserrat', sans-serif;
	}

	/* Typography */
	:global(body) {
		background-color: var(--color-quaternary);
		color: var(--color-grey);
		font-family: var(--font-body);
		font-size: 1.6rem;
		line-height: 1.5;
	}

	:global(h2) {
		color: var(--color-dark);
		font-family: var(--font-heading);
		font-size: 4rem;
		font-weight: normal;
		line-height: 1.2;
	}

	:global(p) {
		font-weight: normal;
	}

	:global(hr) {
		width: 5rem;
		border: 2px solid var(--color-primary);
		margin: 2rem auto;
	}
</style>
