<script>
	import HeaderContact from '$lib/components/HeaderContact.svelte';
	import Navbar from '$lib/components/Navbar.svelte';
</script>

<header>
	<HeaderContact />
	<Navbar />
	<img src="./images/logo-2.png" alt="logo" />
</header>

<style>
	header {
		background: url('ehlen-analytics-heading.jpg') no-repeat center center;
		background-size: cover;
		padding: 20px 0;
		position: relative;
		z-index: 1;
	}

	img {
		width: 15%;
		height: auto;
		display: flex;
		margin: -6rem auto 0 auto;
		padding: 0;
	}
</style>
