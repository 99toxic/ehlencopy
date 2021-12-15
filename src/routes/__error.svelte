<script context="module">
	export const load = ({ error, status }) => {
		return {
			props: {
				error,
				status
			}
		};
	};
</script>

<script>
	import BgVideo from '../lib/components/BgVideo.svelte';
	import HeaderContact from '../lib/components/HeaderContact.svelte';
	import Navbar from '../lib/components/Navbar.svelte';

	export let error;
	export let status;
</script>

<BgVideo />
<div class="overlay">
	<HeaderContact />
	<Navbar />
	<div class="error">
		<h1>{error.name} {status}</h1>
		<p>{error.message}</p>
	</div>
</div>

<style>
	.overlay {
		background-color: var(--color-transparent-black);
		height: 100vh;
		overflow: hidden;
	}
	.error {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 10%;
	}
	h1 {
		color: red;
		text-align: center;
		margin: auto;
		font-size: 8rem;
	}

	p {
		color: blue;
		text-align: center;
		margin: auto;
		font-size: 4rem;
	}
</style>
