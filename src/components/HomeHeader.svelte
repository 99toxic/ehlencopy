<script>
	import BgVideo from './BgVideo.svelte';
	import HeaderContact from './HeaderContact.svelte';
	import Navbar from './Navbar.svelte';

	import HeaderButtons from './HeaderButtons.svelte';
	import HomeHeaderCTA from './HomeHeaderCTA.svelte';
</script>

<header class="header">
	<BgVideo />
	<HeaderContact />
	<Navbar />
	<img class="header-logo" src="../static/images/logo-2.png" alt="logo" />
	<HeaderButtons />
	<HomeHeaderCTA />
</header>

<style>
	.header {
		background-color: var(--color-transparent-black);
		color: var(--color-dark);
		padding: 1.5rem;
		height: 100vh;
		text-align: center;
		position: relative;
	}
	.header-logo {
		width: 33%;
		margin: 0 auto;
		padding: 0;
	}
</style>
