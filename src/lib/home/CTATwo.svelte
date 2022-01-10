<script>
	import ButtonTwo from '$lib/components/ButtonTwo.svelte';
	import Heading from '$lib/components/Heading.svelte';
	let heading = `Ready to get started?`;
	let subHeading = `Contact us today for a free consultation.`;
	let align = `left`;
</script>

<section>
	<Heading {heading} {subHeading} {align} />
	<div class="buttons">
		<ButtonTwo />
	</div>
</section>

<style>
	section {
		background: url('./images/cta-home-rocket.jpg') no-repeat center;
		background-size: fit;
		color: var(--color-tertiary);
		padding: 15rem 10rem;
		margin-bottom: 0;
	}

	.buttons {
		margin-top: 5rem;
	}
</style>
