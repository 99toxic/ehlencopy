<script context="module">
	export const badges = [
		{
			name: 'Facebook Badge',
			image: './images/badges/facebook-badge.png'
		},
		{
			name: 'Google Ads Badge',
			image: './images/badges/google-ads-badge.png'
		},
		{
			name: 'Google Analytics Badge',
			image: './images/badges/google-analytics-badge.png'
		},
		{
			name: 'Google Partner Badge',
			image: './images/badges/google-partner-badge.png'
		},
		{
			name: 'Simrush Badge',
			image: './images/badges/simrush-badge.png'
		},
		{
			name: 'Top Digital Badge',
			image: './images/badges/top-digital-badge.png'
		},
		{
			name: 'Wix Badge',
			image: './images/badges/wix-badge.png'
		}
	];
</script>

<script>
	import { onMount } from 'svelte';

	let Carousel; // for saving Carousel component class
	let carousel; // for calling methods of the carousel instance
	onMount(async () => {
		const module = await import('svelte-carousel');
		Carousel = module.default;
	});

	const handleNextClick = () => {
		carousel.goToNext();
	};
</script>

<section>
	<svelte:component
		this={Carousel}
		bind:this={carousel}
		let:loaded
		autoplay
		autoplayDuration={5000}
		particlesToShow={4}
		particlesToScroll={2}
		arrows={false}
		dots={false}
	>
		{#each badges as badge}
			<div class="badge"><img src={badge.image} alt={badge.name} /></div>
		{/each}
	</svelte:component>
</section>

<style>
	.badge {
		display: flex;
		width: 100%;
		justify-content: center;
		margin: 3rem 0;
	}

	.badge img {
		width: 40rem;
		border: 1px solid var(--color-primary);
		padding: 5rem 10rem;
	}
</style>
