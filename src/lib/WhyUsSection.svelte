<div class="main__why-us">
	<div class="main__why-us__row-1">
		<div class="main__why-us__global-reach main__diamond">
			<i class="fas fa-globe" />
			<h3>Global Reach</h3>
		</div>
		<div class="main__why-us__communication main__diamond">
			<i class="fas fa-users" />
			<h3>Communication</h3>
		</div>
	</div>
	<div class="main__why-us__heading main__diamond">
		<h2>Why Us?</h2>
		<hr />
		<p>
			Ehlen Analytics strives to bring each of our clients individualized, professional digital
			marketing solutions. We use an unmatched level of attention to detail and care with each and
			every project.
		</p>
	</div>
	<div class="main__why-us__row-2">
		<div class="main__why-us__experienced main__diamond">
			<i class="fas fa-briefcase" />
			<h3>Experienced</h3>
		</div>
		<div class="main__why-us__best-practices main__diamond">
			<i class="fas fa-trophy" />
			<h3>Best Practices</h3>
		</div>
		<div class="main__why-us__personalized main__diamond">
			<i class="fas fa-magic" />
			<h3>Personalized</h3>
		</div>
	</div>
</div>

<style>
	.main__why-us {
		background-color: var(--color-tertiary);
	}

	.main__why-us i {
		font-size: 5rem;
	}

	.main__why-us__row-1,
	.main__why-us__row-2 {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}

	.main__why-us__heading {
		margin: 0 auto;
	}

	.main__diamond {
		background: var(--color-secondary);
		height: 40rem;
		transform: rotate(45deg);
		width: 40rem;
	}

	.main__diamond i,
	.main__diamond h2,
	.main__diamond h3,
	.main__diamond hr,
	.main__diamond p {
		transform: rotate(-45deg);
		color: var(--color-white);
	}
</style>
