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
		margin: 0 auto;
		left: 50%;
		transform: translateX(-50%);
		align-items: center;
		color: var(--color-tertiary);
		display: flex;
		font-size: 2rem;
		justify-content: center;
		margin: 5rem 0 20rem 0;
		z-index: 1;
		position: relative;
		width: 70%;
	}

	.cta {
		align-items: center;
		background: var(--color-primary);
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding: 5rem 6rem;
		width: calc(100% / 3);
		height: fit-content;
		position: absolute;
	}

	.cta:nth-child(1) {
		left: 0;
	}

	.cta:nth-child(2) {
		right: 0;
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
		transition: all 0.5s ease-in;
	}
	.cta:hover .text {
		display: block;
		transition: all 5s ease-in-out;
		overflow: hidden;
	}

	@media (max-width: 1100px) {
		section {
			width: 90%;
		}
	}

	@media (max-width: 700px) {
		section {
			width: 100%;
		}
		.cta {
			width: 100%;
		}
	}
</style>
