<div class="header__cta">
	<div class="header-cta__one">
		<i class="fas fa-user" />
		<h4>300+</h4>
		<h5>Happy Clients</h5>
		<div class="header-cta__one__text">
			<p>
				Ehlen Analytics’ #1 goal is customer satisfaction with a high return on their marketing
				dollars.
			</p>
		</div>
	</div>
	<div class="header-cta__two">
		<i class="fas fa-bullhorn" />
		<h4>5+</h4>
		<h5>Years of Experience</h5>
		<div class="header-cta__two__text">
			<p>We have the experience needed to bring your business the results you’re looking for.</p>
		</div>
	</div>
	<div class="header-cta__three">
		<i class="fas fa-clipboard-check" />
		<h4>1,000+</h4>
		<h5>Projects Completed</h5>
		<div class="header-cta__three__text">
			<p>Our quality of work and turnaround time is unmatched in the digital marketing industry.</p>
		</div>
	</div>
</div>

<style>
	.header__cta {
		align-items: center;
		color: var(--color-tertiary);
		display: flex;
		font-size: 2rem;
		justify-content: center;
		padding: 20px;
		position: relative;
		z-index: 1;
	}

	.header-cta__one,
	.header-cta__two,
	.header-cta__three {
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

	.header-cta__one i,
	.header-cta__two i,
	.header-cta__three i {
		font-size: 5rem;
	}

	.header-cta__one h4,
	.header-cta__two h4,
	.header-cta__three h4 {
		font-size: 6rem;
		color: var(--color-white);
	}

	.header-cta__one h5,
	.header-cta__two h5,
	.header-cta__three h5 {
		text-transform: uppercase;
	}

	.header-cta__one__text,
	.header-cta__two__text,
	.header-cta__three__text {
		display: none;
	}

	.header-cta__one:hover,
	.header-cta__two:hover,
	.header-cta__three:hover {
		background: var(--color-secondary);
		transform: translateY(-10rem);
		transition: all 0.5s ease-in-out;
		height: fit-content;
	}

	.header-cta__one:hover .header-cta__one__text,
	.header-cta__two:hover .header-cta__two__text,
	.header-cta__three:hover .header-cta__three__text {
		display: inline-block;
		opacity: 1;
		transition: all 0.5s ease-in-out;
	}
</style>
