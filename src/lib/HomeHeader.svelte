<script>
	import BgVideo from '$lib/BgVideo.svelte';
	import HeaderContact from '$lib/HeaderContact.svelte';
	import Navbar from '$lib/Navbar.svelte';

	import HeaderButtons from '$lib/HeaderButtons.svelte';
</script>

<header>
	<BgVideo />
	<HeaderContact />
	<Navbar />
	<img src="../static/images/logo-2.png" alt="logo" />
	<h2>Dominate your market</h2>
	<HeaderButtons />
</header>

<style>
	header {
		background-color: var(--color-transparent-black);
		color: var(--color-dark);
		padding: 2rem 5rem;
		height: 100vh;
		text-align: center;
		position: relative;
	}
	img {
		width: 585px;
		margin: 0 auto;
		margin-top: 8%;
		display: block;
	}
	h2 {
		color: var(--color-white);
		margin-top: -4rem;
		margin-bottom: 3rem;
	}
</style>
