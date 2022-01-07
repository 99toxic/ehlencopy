<script context="module">
	export const testimonials = [
		{
			image: '',
			name: 'David P',
			description:
				'Ehlen Analytics has changed my business forever. Their marketing team has changed everything. We went from not having any jobs to booking up three weeks in advance. They know what they’re doing. If you’re on the ropes about should I go with them, should I not… DO IT! It’ll change your life.'
		}
	];
</script>

<script>
	import Heading from '$lib/components/Heading.svelte';
	import { onMount } from 'svelte';

	let heading = 'Testimonials';
	let subHeading = 'Real clients. Real reviews.';
	let align = 'center';

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
	<Heading {heading} {subHeading} {align} />

	<svelte:component
		this={Carousel}
		bind:this={carousel}
		let:loaded
		autoplay
		autoplayDuration={5000}
		particlesToShow={2}
		particlesToScroll={2}
		arrows={false}
		dots={false}
	>
		{#each testimonials as testimonial}
			<div class="wrap">
				<div class="testimonial">
					<div class="content">
						<p>{testimonial.description}</p>
					</div>
					<div class="name">
						<img src={testimonial.image} alt={testimonial.name} />
						<p class="name">{testimonial.name}</p>
					</div>
				</div>
			</div>
		{/each}
	</svelte:component>
</section>

<style>
	section {
		background: url('../images/services-background.png') no-repeat left top;
		background-size: fit;
	}

	.wrap {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		margin: 0 auto;
		max-width: 1200px;
		padding: 0;
		margin-bottom: 20rem;
	}

	.testimonial {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 0 auto;
		max-width: 600px;
		padding: 0;
	}

	.content {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		margin: 0 auto;
		max-width: 600px;
		padding: 0;
	}

	.content p {
		margin: 0;
		padding: 0;
		font-size: 1.5rem;
	}
</style>
