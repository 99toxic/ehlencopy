<div class="why-us">
	<div class="row-1">
		<div class="global-reach diamond">
			<i class="fas fa-globe" />
			<h3>Global Reach</h3>
		</div>
		<div class="communication diamond">
			<i class="fas fa-users" />
			<h3>Communication</h3>
		</div>
	</div>
	<div class="heading diamond">
		<h2>Why Us?</h2>
		<hr />
		<p>
			Ehlen Analytics strives to bring each of our clients individualized, professional digital
			marketing solutions. We use an unmatched level of attention to detail and care with each and
			every project.
		</p>
	</div>
	<div class="row-2">
		<div class="experienced diamond">
			<i class="fas fa-briefcase" />
			<h3>Experienced</h3>
		</div>
		<div class="best-practices diamond">
			<i class="fas fa-trophy" />
			<h3>Best Practices</h3>
		</div>
		<div class="personalized diamond">
			<i class="fas fa-magic" />
			<h3>Personalized</h3>
		</div>
	</div>
</div>

<style>
	.why-us {
		background-color: var(--color-tertiary);
		margin-top: 10rem;
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
		/* put items in middle */
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 0 auto;
		transform: rotate(45deg);
	}

	.heading {
		background: var(--color-primary);
		height: 40rem;
		width: 40rem;
	}

	.row-1 .diamond {
		background: var(--color-secondary);
		height: 20rem;
		margin: -5rem 20rem 0 20rem;
		text-align: center;
		transform: rotate(45deg);
		width: 20rem;
	}

	.row-2 .diamond {
		background: var(--color-secondary);
		height: 20rem;
		margin: 5rem 20rem -5rem 20rem;
		text-align: center;
		transform: rotate(45deg);
		width: 20rem;
	}

	.heading {
		text-align: center;
		margin: 0 auto;
		margin-bottom: 50px;
	}

	h2 {
		font-size: 2.5rem;
		font-weight: 700;
		margin-bottom: 20px;
	}

	h3 {
		font-size: 1.5rem;
		font-weight: 700;
		margin-bottom: 20px;
	}

	hr {
		width: 50px;
		height: 2px;
		background-color: #000;
		margin: 0 auto;
		margin-bottom: 30px;
	}

	i,
	h2,
	h3,
	hr,
	p {
		transform: rotate(-45deg);
		color: var(--color-white);
	}

	i {
		font-size: 3rem;
		margin-bottom: 20px;
	}
</style>
