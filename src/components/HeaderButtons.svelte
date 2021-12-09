<div class="header-buttons">
	<a class="header-buttons__call" href="tel:8284923347"><i class="fas fa-phone-volume" />Call Now</a
	>
	<a class="header-buttons__contact" href="/contact">Contact Us</a>
</div>

<style>
	.header-buttons {
		display: flex;
		justify-content: space-evenly;
		align-items: center;
		padding: 1rem;
		width: 50%;
		margin: 0 auto 10rem auto;
	}

	.header-buttons__call,
	.header-buttons__contact {
		font-size: 2rem;
		color: var(--color-tertiary);
		margin-right: 1rem;
		text-decoration: none;
		padding: 0.8rem 3rem;
		border-radius: 5rem;
	}

	.header-buttons__call {
		border: 2px solid var(--color-primary);
		color: var(--color-primary);
	}

	.header-buttons__call:hover {
		background-color: var(--color-primary);
		color: var(--color-white);
	}

	.header-buttons__call i {
		margin-right: 1rem;
		font-size: 2rem;
	}

	.header-buttons__contact {
		background: var(--color-gradient-primary);
	}

	.header-buttons__contact:hover {
		background: var(--color-secondary);
	}
</style>
