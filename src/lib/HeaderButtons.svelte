<div class="header-buttons">
	<a class="header-buttons__call" href="tel:8284923347"><i class="fas fa-phone-volume" />Call Now</a
	>
	<a class="header-buttons__contact" href="/contact">Contact Us</a>
</div>

<style>
	.header-buttons {
		align-items: center;
		display: flex;
		justify-content: space-evenly;
		margin: 0 auto;
		width: 40%;
	}

	.header-buttons__call,
	.header-buttons__contact {
		border-radius: 5rem;
		color: var(--color-tertiary);
		font-size: 2rem;
		font-weight: 700;
		margin-top: 1.5rem;
		padding: 2rem 3.5rem;
		text-decoration: none;
		text-transform: uppercase;
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
		font-size: 2rem;
		margin-right: 0.5rem;
	}

	.header-buttons__contact {
		background: var(--color-gradient-primary);
	}

	.header-buttons__contact:hover {
		background: var(--color-secondary);
	}
</style>
