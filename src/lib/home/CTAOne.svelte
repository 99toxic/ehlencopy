<script>
	import ButtonTwo from '$lib/components/ButtonTwo.svelte';
	import ButtonThree from '$lib/components/ButtonThree.svelte';
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Start Boosting Your Rankings Today!';
	let subHeading = `We can’t wait to help you Dominate Your Market. All of our clients get personalized projects
			because we know that there’s no one-size-fits-all optimization. Experience the difference that
			superior digital marketing makes.`;
	let align = 'left';
</script>

<section>
	<Heading {heading} {subHeading} {align} />
	<div class="buttons">
		<ButtonTwo />
		<ButtonThree />
	</div>
</section>

<style>
	section {
		background: url('./static/images/main-cta-1-bg.jpg') no-repeat center;
		background-size: cover;
		color: var(--color-tertiary);
		padding: 15rem 10rem;
		margin-bottom: 0;
	}
	.buttons {
		align-items: center;
		margin-top: 5rem;
	}
</style>
