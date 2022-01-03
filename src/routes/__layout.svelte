<script>
	// import HomeHeader from '$lib/HomeHeader.svelte';
	// import MainHeader from '$lib/MainHeader.svelte';
</script>

<svelte:head>
	<!-- Google Fonts -->
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Raleway&display=swap"
		rel="stylesheet"
	/>

	<!-- Font-Awesome -->
	<link
		rel="stylesheet"
		href="https://use.fontawesome.com/releases/v5.0.13/css/all.css"
		integrity="sha384-DNOHZ68U8hZfKXOrtjWvjxusGo9WQnrNx2sqG0tfsghAvtVlRW3tvkXWZh58N9jp"
		crossorigin="anonymous"
	/>
</svelte:head>

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
</style>
