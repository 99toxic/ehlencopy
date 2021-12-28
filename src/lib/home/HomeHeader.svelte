<script>
	import BgVideo from '$lib/components/BgVideo.svelte';
	import HeaderContact from '$lib/components/HeaderContact.svelte';
	import Navbar from '$lib/components/Navbar.svelte';

	import HeaderButtons from '$lib/components/HeaderButtons.svelte';
</script>

<header>
	<BgVideo />
	<HeaderContact />
	<Navbar />
	<div class="logo">
		<img src="../../static/images/logo-2.png" alt="logo" />
		<h2>Dominate Your Market</h2>
		<HeaderButtons />
	</div>
</header>

<style>
	header {
		background-color: var(--color-transparent-black);
		color: var(--color-dark);
		height: 100vh;
		padding: 2rem 5rem;
		position: relative;
		text-align: center;
	}

	.logo {
		left: 50%;
		position: absolute;
		top: 50%;
		transform: translate(-50%, -50%);
		width: 100%;
	}
	img {
		display: block;
		margin: 0 auto;
		width: 30%;
	}
	h2 {
		color: var(--color-white);
		font-size: 4.5rem;
		margin-bottom: 2rem;
		margin-top: -3.5rem;
	}
</style>
