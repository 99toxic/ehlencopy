<section>
	<div class="cta">
		<i class="fas fa-user" />
		<h4>300+</h4>
		<h5>Happy Clients</h5>
		<div class="text">
			<p>
				Ehlen Analytics’ #1 goal is customer satisfaction with a high return on their marketing
				dollars.
			</p>
		</div>
	</div>
	<div class="cta">
		<i class="fas fa-bullhorn" />
		<h4>5+</h4>
		<h5>Years of Experience</h5>
		<div class="text">
			<p>We have the experience needed to bring your business the results you’re looking for.</p>
		</div>
	</div>
	<div class="cta">
		<i class="fas fa-clipboard-check" />
		<h4>1,000+</h4>
		<h5>Projects Completed</h5>
		<div class="text">
			<p>Our quality of work and turnaround time is unmatched in the digital marketing industry.</p>
		</div>
	</div>
</section>

<style>
	section {
		align-items: center;
		color: var(--color-tertiary);
		display: flex;
		font-size: 2rem;
		justify-content: center;
		padding: 20px;
		position: relative;
		z-index: 1;
	}

	.cta {
		align-items: center;
		background: var(--color-primary);
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding: 4rem 6rem;
		width: 40rem;
		height: 30rem;
		margin-top: -10rem;
	}

	i {
		font-size: 5rem;
	}

	h4 {
		font-size: 6rem;
		color: var(--color-white);
	}

	h5 {
		text-transform: uppercase;
	}

	.text {
		display: none;
	}

	.cta:hover {
		background: var(--color-secondary);
		transform: translateY(-10rem);
		transition: all 0.5s ease-in-out;
		height: fit-content;
	}
	.cta:hover .text {
		display: inline-block;
		opacity: 1;
		transition: all 0.5s ease-in-out;
	}
</style>
