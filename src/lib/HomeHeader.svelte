<script>
	import BgVideo from '$lib/BgVideo.svelte';
	import HeaderContact from '$lib/HeaderContact.svelte';
	import Navbar from '$lib/Navbar.svelte';

	import HeaderButtons from '$lib/HeaderButtons.svelte';
</script>

<header class="header">
	<BgVideo />
	<HeaderContact />
	<Navbar />
	<img class="header-logo" src="../static/images/logo-2.png" alt="logo" />
	<HeaderButtons />
</header>

<style>
	.header {
		background-color: var(--color-transparent-black);
		color: var(--color-dark);
		padding: 2rem 5rem;
		height: 100vh;
		text-align: center;
		position: relative;
	}
	.header-logo {
		width: 35%;
		margin: 0 auto;
		margin-top: 8%;
		display: block;
	}
</style>
