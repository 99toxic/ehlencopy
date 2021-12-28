<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Why Us';
	let subHeading = `Ehlen Analytics strives to bring each of our clients individualized, professional digital
				marketing solutions. We use an unmatched level of attention to detail and care with each and
				every project.`;
</script>

<section>
	<div class="row-1">
		<div class="global-reach diamond">
			<div class="rotate">
				<i class="fas fa-globe" />
				<h3>Global Reach</h3>
			</div>
		</div>
		<div class="communication diamond">
			<div class="rotate">
				<i class="fas fa-users" />
				<h3>Communication</h3>
			</div>
		</div>
	</div>
	<div class="heading diamond">
		<div class="rotate">
			<Heading {heading} {subHeading} />
		</div>
	</div>
	<div class="row-2">
		<div class="experienced diamond">
			<div class="rotate">
				<i class="fas fa-briefcase" />
				<h3>Experienced</h3>
			</div>
		</div>
		<div class="best-practices diamond">
			<div class="rotate">
				<i class="fas fa-trophy" />
				<h3>Best Practices</h3>
			</div>
		</div>
		<div class="personalized diamond">
			<div class="rotate">
				<i class="fas fa-magic" />
				<h3>Personalized</h3>
			</div>
		</div>
	</div>
</section>

<style>
	section {
		background-color: var(--color-tertiary);
		margin-top: 20rem;
	}

	.rotate {
		transform: rotate(-45deg);
	}

	.row-1 {
		display: flex;
		justify-content: center;
		margin-bottom: 50px;
	}

	.row-2 {
		display: flex;
		justify-content: space-between;
		margin-bottom: 50px;
	}

	.diamond {
		display: flex;
		flex-direction: column;
		justify-content: center;
		margin: 0 auto;
		transform: rotate(45deg);
	}

	.heading {
		background: var(--color-white);
		height: 40rem;
		margin-bottom: 50px;
		text-align: center;
		width: 40rem;
	}

	.row-1 .diamond {
		background: var(--color-secondary);
		height: 20rem;
		margin: -5rem 20rem 0 20rem;
		text-align: center;
		width: 20rem;
	}

	.row-2 .diamond {
		background: var(--color-secondary);
		height: 20rem;
		margin: 5rem 20rem -5rem 20rem;
		text-align: center;
		width: 20rem;
	}

	h3 {
		font-size: 1.5rem;
		font-weight: 700;
		margin-bottom: 20px;
		color: var(--color-white);
	}

	hr {
		width: 50px;
		height: 2px;
		background-color: #000;
		margin: 30px auto;
	}

	i {
		font-size: 3rem;
		margin-bottom: 20px;
		color: var(--color-white);
	}
</style>
