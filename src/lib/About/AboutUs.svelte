<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'About Us';
	let subHeading = 'Founded by two brothers with a passion for digital marketing';
	let align = 'center';
</script>

<section>
	<Heading {heading} {subHeading} {align} />
	<div class="wrap">
		<main>
			<p>
				Ehlen Analytics was founded in 2017 by brothers Daniel and Matthew Ehlen after Daniel left
				another agency to start his own, seeing what they were lacking and hoping to exceed
				expectations. What started as a basement operation quickly became an astronomical success,
				as it became increasingly apparent that our digital marketing strategies were just what
				business owners across the globe were looking for.
			</p>

			<p>
				Today, our company continues to operate with the goal of helping our clients get the most
				out of their digital marketing experience. We offer personalized campaigns for every client,
				never settling for one-size-fits-all solutions.
			</p>

			<p>We can’t wait to work with you!</p>
		</main>

		<div class="image">
			<img src="../static/images/team/matthew-ehlen.jpg" alt="services" />
			<img src="../static/images/team/daniel-ehlen.jpg" alt="services" />
		</div>
	</div>
</section>

<style>
	.wrap {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		align-items: center;
		padding: 10rem;
	}

	.image {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		align-items: center;
		gap: 3rem;
	}
</style>
