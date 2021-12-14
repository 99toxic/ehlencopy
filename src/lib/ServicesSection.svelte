<script>
	import Heading from '$lib/Heading.svelte';
	import { services } from '../stores/services';

	let heading = 'Our digital marketing services';
	let subHeading =
		'Our services are uniquely optimized for each individual client, to best suit your needs.';
</script>

<Heading {heading} {subHeading} />

<div class="services">
	<div class="image">
		<img src="images/iphone.jpg" alt="services" />
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

<style>
	.services {
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
</style>
