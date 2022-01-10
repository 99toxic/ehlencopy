<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Why Us';
	let subHeading = `Ehlen Analytics strives to bring each of our clients individualized, professional digital
				marketing solutions. We use an unmatched level of attention to detail and care with each and
				every project.`;
	let align = 'center';
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
			<Heading {heading} {subHeading} {align} />
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
		background: url('../images/whyus-background.jpg') no-repeat 50% 100%;
		background-size: cover;
		margin-top: 20rem;
	}

	.rotate {
		transform: rotate(-45deg);
	}

	.row-1 {
		display: flex;
		justify-content: space-between;
	}

	.row-2 {
		display: flex;
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
		height: 41rem;
		margin-bottom: 50px;
		text-align: center;
		width: 41rem;
	}

	.row-1 .diamond,
	.row-2 .diamond {
		background: var(--color-secondary);
		text-align: center;
	}

	.global-reach {
		position: relative;
		bottom: -15rem;
		height: 21rem;
		right: -30rem;
		z-index: 9;
		width: 21rem;
	}

	.communication {
		height: 24rem;
		width: 24rem;
	}

	.best-practices {
		position: relative;
		top: -4rem;
		left: -15rem;
		height: 21rem;
		width: 21rem;
	}

	.experienced {
		position: relative;
		top: -30rem;
		height: 22rem;
		width: 22rem;
	}

	.personalized {
		position: relative;
		top: -20rem;
		height: 24rem;
		width: 24rem;
	}

	h3 {
		color: var(--color-white);
	}

	i {
		font-size: 5rem;
		margin-bottom: 20px;
		color: var(--color-white);
	}
</style>
