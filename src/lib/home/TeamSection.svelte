<script context="module">
	export const teamMember = [
		{
			image: '../static/images/team/nick-simpson.jpg',
			name: 'Nick Simpson',
			position: 'Web Developer & Designer',
			description:
				'Nick is a UX / UI Designer and Web Developer with an entrepreneurial spirit and a passion for user-centric design.',
			facebook: 'https://www.facebook.com/profile.php?id=100070518892846',
			twitter: 'https://twitter.com/99toxic',
			linkedin: 'https://www.linkedin.com/in/jamesnsimpson/'
		},
		{
			image: '../static/images/team/michael-ehlen.jpg',
			name: 'Michael Ehlen',
			position: 'Sales Associate',
			description:
				'Michael offers business consulting to potential clients. Our sales team is dedicated to matching your digital marketing needs with our services.',
			facebook: 'https://www.facebook.com/mike.ehlen.90',
			linkedin: 'https://www.linkedin.com/in/michael-ehlen-b38a0a21a/'
		},
		{
			image: '../static/images/team/josh-titherington.jpg',
			name: 'Josh Titherington',
			position: 'PPC Specialist',
			description:
				'Joshua analyzes and deploys Facebook and Google Pay Per Click campaigns that are optimized individually for maximum client success.',
			facebook: 'https://www.facebook.com/profile.php?id=100073113433832',
			linkedin: ''
		},
		{
			image: '../static/images/team/Laney-Poff-1.jpg',
			name: 'Laney Poff',
			position: 'SEO Specialist',
			description:
				'Laney analyzes and optimizes client websites and other digital properties to improve visibility in search results and drive traffic to their site.',
			facebook:
				'https://www.facebook.com/profile.php?id=100070116883116" tabindex="0"><i class="icon-facebook',
			linkedin: ''
		}
	];
</script>

<script>
	// import Carousel from 'svelte-carousel';
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Our Team';
	let subHeading =
		'Unlike most digital marketing agencies, all of our employees work in-house. In our office, collaboration and communication are a key focus every single day.';
	let align = 'center';

	import { onMount } from 'svelte';

	let Carousel; // for saving Carousel component class
	let carousel; // for calling methods of the carousel instance
	onMount(async () => {
		const module = await import('svelte-carousel');
		Carousel = module.default;
	});

	const handleNextClick = () => {
		carousel.goToNext();
	};
</script>

<section>
	<Heading {heading} {subHeading} {align} />
	<svelte:component
		this={Carousel}
		bind:this={carousel}
		autoplay
		autoplayDuration={5000}
		particlesToShow={2}
		particlesToScroll={2}
		arrows={false}
	>
		{#each teamMember as team}
			<div class="wrap">
				<div class="team-member">
					<div class="team-member-image">
						<img src={team.image} alt={team.name} />
					</div>
					<div class="team-member-info">
						<h3>{team.name}</h3>
						<p class="position">{team.position}</p>
						<p class="description">{team.description}</p>
						<!-- add socail links -->
						<div class="social-links">
							<a href={team.facebook} target="_blank"><i class="fab fa-facebook-f" /></a>
							<a href={team.twitter} target="_blank"><i class="fab fa-twitter" /></a>
							<a href={team.linkedin} target="_blank"><i class="fab fa-linkedin" /></a>
						</div>
					</div>
				</div>
			</div>
		{/each}
	</svelte:component>
</section>

<style>
	section {
		background: url('../images/team.jpg') no-repeat center top;
		background-size: fit;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		color: var(--color-white);
	}

	.wrap {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 0;
	}
	.team-member {
		margin: 10rem 2rem;
		display: flex;
		flex-direction: row;
		align-items: top;
		justify-content: space-around;
		width: 30%;
		background-color: var(--color-white);
		color: var(--color-black);
		box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
	}

	.team-member-info {
		padding: 2rem;
	}

	.position {
		font-size: 1.5rem;
		font-weight: 700;
	}

	.description {
		font-size: 1.2rem;
		margin-top: 1rem;
	}

	.social-links {
		display: flex;
		justify-content: flex-start;
		margin-top: 1rem;
	}

	.social-links a {
		margin-right: 1rem;
	}

	.social-links a i {
		font-size: 1.5rem;
		color: var(--color-black);
	}
</style>
