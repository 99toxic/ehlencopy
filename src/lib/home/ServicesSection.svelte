<script context="module">
	export const services = [
		{
			title: 'Google Ads',
			description:
				'We expertly optimize your Google Ads to target primary customers, so you can get the most out of your budget.',
			icon: 'fab fa-google',
			link: '/google-ads'
		},
		{
			title: 'Reputation Management Services',
			description:
				'We monitor your online reputation to make it appealing to potential customers by improving your ratings and presence.',
			icon: 'fas fa-star',
			link: '/reputation-management'
		},
		{
			title: 'Google My Business',
			description:
				'We will set up, fully develop, and continuously update your GMB to ensure your business is relevant and ranking on the SERP.',
			icon: 'fas fa-map-marker-alt',
			link: '/google-my-business'
		},
		{
			title: 'Facebook Ads',
			description:
				'We professionally personalize all Facebook Ads in order to make them eye-catching and appealing to potential customers.',
			icon: 'fab fa-facebook-f',
			link: '/facebook-ads'
		},
		{
			title: 'Web Design & Development',
			description:
				'We create beautiful, fast, efficient websites that are interesting and informative, so you get the most out of your investment.',
			icon: 'fas fa-laptop',
			link: '/web-design-development'
		},
		{
			title: 'Local & National SEO',
			description:
				'We complete full SEO on your website and GMB, during and after they are built, to ensure that your rankings continue to grow',
			icon: 'fas fa-search',
			link: '/local-national-seo'
		},
		{
			title: 'Social Media Management',
			description:
				'We build a personalized posting schedule, to brand your business’s social media accounts and keep them relevant.',
			icon: 'fas fa-users',
			link: '/social-media-management'
		},
		{
			title: 'Content Writing',
			description:
				'We have experienced in-house content writers who are fully trained to optimize your website, GMB, and social media content.',
			icon: 'fas fa-pencil-alt',
			link: '/content-writing'
		}
	];
</script>

<script>
	import HomeHeaderCTA from '$lib/home/HomeHeaderCTA.svelte';
	import Heading from '$lib/components/Heading.svelte';

	let heading = 'Our digital marketing services';
	let subHeading =
		'Our services are uniquely optimized for each individual client, to best suit your needs.';
	let align = 'center';
</script>

<section>
	<HomeHeaderCTA />
	<Heading {heading} {subHeading} {align} />
	<div class="main">
		<div class="image">
			<img src="./images/iphone.jpg" alt="services" />
		</div>
		<div class="wrap">
			{#each services as service}
				<div class="item">
					<div class="item__icon">
						<i class={service.icon} />
					</div>
					<div class="item__text">
						<h3>{service.title}</h3>
						<p>
							{service.description}
						</p>
						<a href={service.link}>Read More</a>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>

<style>
	section {
		background: url('./images/services-background.png') no-repeat left top;
	}
	.main {
		display: flex;
		margin-top: 5rem;
		justify-content: space-evenly;
	}

	.image {
		width: 400px;
	}

	.image img {
		width: 100%;
	}

	.wrap {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		width: 50%;
	}

	.item {
		display: flex;
		width: 35rem;
		margin: 4rem 0;
	}

	.item__icon {
		font-size: 4rem;
		color: var(--color-primary);
		margin-right: 4rem;
	}

	.item__text {
		display: flex;
		flex-direction: column;
	}

	.item a {
		font-size: 1.5rem;
		color: var(--color-grey);
		text-decoration: none;
		text-transform: uppercase;
		font-weight: bold;
		margin-top: 2rem;
		text-align: right;
		visibility: hidden; /* //& Hide the link text until hover */
	}

	@media only screen and (max-width: 1100px) {
		.image {
			display: none;
		}

		.wrap {
			width: 100%;
		}
	}
</style>
