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
	let heading = 'Testimonials';
	let subHeading = 'Real clients. Real reviews.';
	let align = 'center';
</script>

<section>
	<Heading {heading} {subHeading} {align} />

	<div class="wrap">
		{#each testimonials as testimonial}
			<div class="testimonial">
				<div class="testimonial__image">
					<img src={testimonial.image} alt={testimonial.name} />
				</div>
				<div class="testimonial__content">
					<p>{testimonial.description}</p>
					<p class="testimonial__name">{testimonial.name}</p>
				</div>
			</div>
		{/each}
	</div>
</section>

<style>
	section {
		background: url('../images/services-background.png') no-repeat left top;
		background-size: fit;
	}
</style>
