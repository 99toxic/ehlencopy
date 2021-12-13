<div class="main__services">
	<div class="main__services__image">
		<img src="images/iphone.jpg" alt="services" />
	</div>
	<div class="main__services__wrap">
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fab fa-google" />
			</div>
			<div class="main__services__item__text">
				<h3>Google Ads</h3>
				<p>
					We expertly optimize your Google Ads to target primary customers, so you can get the most
					out of your budget.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fas fa-star" />
			</div>
			<div class="main__services__item__text">
				<h3>Reputation Management Services</h3>
				<p>
					We monitor your online reputation to make it appealing to potential customers by improving
					your ratings and presence.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fas fa-search" />
			</div>
			<div class="main__services__item__text">
				<h3>Google My Business</h3>
				<p>
					We will set up, fully develop, and continuously update your GMB to ensure your business is
					relevant and ranking on the SERP.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fab fa-facebook-f" />
			</div>
			<div class="main__services__item__text">
				<h3>Facebook Ads</h3>
				<p>
					We professionally personalize all Facebook Ads in order to make them eye-catching and
					appealing to potential customers.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="far fa-window-maximize" />
			</div>
			<div class="main__services__item__text">
				<h3>Web Design / development</h3>
				<p>
					We create beautiful, fast, efficient websites that are interesting and informative, so you
					get the most out of your investment.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>

		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fas fa-search" />
			</div>
			<div class="main__services__item__text">
				<h3>Local & National SEO</h3>
				<p>
					We complete full SEO on your website and GMB, during and after they are built, to ensure
					that your rankings continue to grow.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="fas fa-users" />
			</div>
			<div class="main__services__item__text">
				<h3>Social Media Management</h3>
				<p>
					We build a personalized posting schedule, to brand your business’s social media accounts
					and keep them relevant.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
		<div class="main__services__item">
			<div class="main__services__item__icon">
				<i class="far fa-edit" />
			</div>
			<div class="main__services__item__text">
				<h3>Content Writing</h3>
				<p>
					We have experienced in-house content writers who are fully trained to optimize your
					website, GMB, and social media content.
				</p>
				<a href="#">Read More</a>
			</div>
		</div>
	</div>
</div>

<style>
	.main__services {
		display: flex;
		margin-top: 5rem;
		justify-content: space-evenly;
	}

	.main__services__image {
		width: 400px;
	}

	.main__services__image img {
		width: 100%;
	}

	.main__services__wrap {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		width: 50%;
	}

	.main__services__item {
		display: flex;
		width: 35rem;
		margin: 4rem 0;
	}

	.main__services__item__icon {
		font-size: 4rem;
		color: var(--color-primary);
		margin-right: 4rem;
	}

	.main__services__item__text {
		display: flex;
		flex-direction: column;
	}

	.main__services__item a {
		font-size: 1.5rem;
		color: var(--color-grey);
		text-decoration: none;
		text-transform: uppercase;
		font-weight: bold;
		margin-top: 2rem;
		text-align: right;
		visibility: hidden; /* //& Hide the link text until hover */
	}
</style>
