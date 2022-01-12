<script>
	// import HomeHeader from '$lib/HomeHeader.svelte';
	// import MainHeader from '$lib/MainHeader.svelte';
	import '../styles/global.css';
	import Footer from '$lib/components/Footer.svelte';
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

<Footer />

<!-- {#if }
	<HomeHeader />
{:else}
	<MainHeader />
{/if} -->
