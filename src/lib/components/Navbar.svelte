<div class="navbar">
	<div class="navbar__logo">
		<a href="index.html">
			<img src="../static/logo.png" alt="logo" />
		</a>
	</div>
	<div class="navbar__menu">
		<nav>
			<ul>
				<li><a class="home" href="/">Home</a></li>
				<li><a href="/about">About</a></li>
				<li><a href="/services">Services</a></li>
				<li><a href="/support-forms">Support Forms</a></li>
				<li><a href="/contact">Contact Us</a></li>
			</ul>
		</nav>
	</div>
</div>

<style>
	.navbar {
		display: flex;
		justify-content: flex-end;
		padding: 0px;
	}

	.navbar__logo {
		display: none; /* //# hide logo  (show for fixed navigation) */
	}

	.navbar__menu nav ul {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.navbar__menu nav ul li {
		display: flex;
		align-items: center;
		justify-content: center;
		margin-right: 1rem;
	}

	.navbar__menu nav ul li a {
		font-size: 1.5rem;
		color: var(--color-tertiary);
		margin-right: 1rem;
		text-decoration: none;
		text-transform: uppercase;
		font-weight: bold;
	}

	.navbar__menu nav ul li a:hover {
		color: var(--color-primary);
	}

	/* //# Add active class to navigation when on page */
	/* .active {
		color: var(--color-secondary);
	} */
</style>
