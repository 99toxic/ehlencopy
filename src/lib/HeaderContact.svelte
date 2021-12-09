<div class="header-contact">
	<div class="header-contact__icons">
		<a href="https://www.facebook.com/EhlenAnalytics/"><i class="fab fa-facebook-f" /></a>
		<a href="https://twitter.com/ehlenanalytics?lang=en"><i class="fab fa-twitter" /></a>
		<a href="https://www.linkedin.com/company/ehlen-analytics/mycompany/"
			><i class="fab fa-linkedin-in" /></a
		>
		<a href="https://www.instagram.com/ehlenanalytics/?hl=en"><i class="fab fa-instagram" /></a>
	</div>
	<div class="header-contact__text">
		<a href="mailto:help@ehlenanalytics.net"><i class="fas fa-envelope" />help@ehlenanalytics.net</a
		>
		<a href="tel:828-974-6408"><i class="fas fa-phone-volume" />(828) 974-6408</a>
	</div>
</div>

<style>
	.header-contact {
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 0.5rem;
		width: 100%;
		padding: 1rem;
	}

	.header-contact__icons {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.header-contact__icons i {
		font-size: 1.5rem;
		color: var(--color-tertiary);
		margin-right: 1rem;
		background-color: var(--color-transparent-background);
		padding: 1rem;
		border-radius: 50%;
	}

	.header-contact__icons i:hover {
		background-color: var(--color-primary);
		color: var(--color-white);
	}

	.header-contact__text a {
		font-size: 1.5rem;
		color: var(--color-tertiary);
		text-decoration: none;
	}

	.header-contact__text a:not(:last-child) {
		margin-right: 1rem;
	}

	.header-contact__text i {
		font-size: 1.5rem;
		margin-right: 1rem;
	}
</style>
