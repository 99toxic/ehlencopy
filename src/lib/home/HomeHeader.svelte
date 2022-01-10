<script>
	import BgVideo from '$lib/components/BgVideo.svelte';
	import HeaderContact from '$lib/components/HeaderContact.svelte';
	import Navbar from '$lib/components/Navbar.svelte';

	import ButtonOne from '$lib/components/ButtonOne.svelte';
	import ButtonTwo from '$lib/components/ButtonTwo.svelte';
</script>

<header>
	<BgVideo />
	<HeaderContact />
	<Navbar />
	<div class="logo">
		<img src="./images/logo-2.png" alt="logo" />
		<h2>Dominate Your Market</h2>
		<div class="buttons">
			<ButtonOne />
			<ButtonTwo />
		</div>
	</div>
</header>

<style>
	header {
		background-color: var(--color-transparent-black);
		color: var(--color-dark);
		height: 100vh;
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
		min-width: 350px;
	}
	h2 {
		color: var(--color-white);
	}
	.buttons {
		align-items: center;
		display: flex;
		justify-content: space-evenly;
		margin: 0 auto;
		width: 40%;
	}
</style>
