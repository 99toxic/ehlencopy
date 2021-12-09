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
		margin: 0;
		padding: 0;
		box-sizing: inherit;
	}

	:global(html) {
		box-sizing: border-box;
		font-size: 62.5%; /* 10px / 16px = 62.5% -> 1rem = 10px */
	}

	/* Variables */
	:root {
		--color-primary: #1aad92;
		--color-secondary: #1b56e9;
		--color-tertiary: #f2f2f3;
		--color-white: #fff;
		--color-black: #000;
		--color-black-2: #252a2c;

		--color-transparent-white: rgba(255, 255, 255, 0.13);
		--color-transparent-black: rgba(0, 0, 0, 0.7);

		--color-gradient-primary: linear-gradient(to right, #1b56e9 0%, #1aad92 100%);

		--font-body: 'Raleway', sans-serif;
		--font-heading: 'Montserrat', sans-serif;
	}

	/* Typography */
	:global(body) {
		font-family: var(--font-body);
		font-size: 1.6rem;
		line-height: 1.5;
		color: var(--color-grey);
		background-color: var(--color-quaternary);
	}

	:global(h2) {
		font-family: var(--font-heading);
		color: var(--color-dark);
		font-size: 5rem;
		font-weight: normal;
		line-height: 1.2;
	}

	:global(p) {
		font-size: 1.6rem;
		font-weight: normal;
	}

	:global(hr) {
		width: 5rem;
		border: 2px solid var(--color-primary);
		margin: 2rem auto;
	}
</style>
