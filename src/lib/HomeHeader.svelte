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
	<div class="logo">
		<img src="../static/images/logo-2.png" alt="logo" />
		<h2>Dominate your market</h2>
		<HeaderButtons />
	</div>
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

	.logo {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
		width: 100%;
	}
	img {
		margin: 0 auto;
		width: 30%;
		display: block;
	}
	h2 {
		color: var(--color-white);
		margin-top: -2rem;
		margin-bottom: 2rem;
		font-size: 2.5rem;
	}
</style>
