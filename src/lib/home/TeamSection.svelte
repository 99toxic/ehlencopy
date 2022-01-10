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
			image: '../static/images/team/Laney-Poff.jpg',
			name: 'Laney Poff',
			position: 'SEO Specialist',
			description:
				'Laney analyzes and optimizes client websites and other digital properties to improve visibility in search results and drive traffic to their site.',
			facebook:
				'https://www.facebook.com/profile.php?id=100070116883116" tabindex="0"><i class="icon-facebook',
			linkedin: ''
		},
		{
			image: '../static/images/team/maryanne-morgan.jpg',
			name: 'Maryanne Morgan',
			position: 'Media & Content Specialist',
			description:
				'Maryanne writes optimized content for our Web Design and Social Media clients and creates personalized graphic designs.',
			facebook: 'https://www.facebook.com/profile.php?id=100064136550894',
			linkedin: 'https://www.linkedin.com/in/maryanne-morgan-9833b456/'
		},
		{
			image: '../static/images/team/brittney-caggige.jpg',
			name: 'Brittney Caggige',
			position: 'Admin',
			description:
				'Brittney ensures that all clients are well cared for, up to date, and receiving a systematic approach that guarantees them success.',
			facebook: 'https://www.facebook.com/profile.php?id=100069099465690',
			linkedin: 'https://www.linkedin.com/in/brittney-caggige-8566b4214/'
		},
		{
			image: '../static/images/team/matthew-ehlen.jpg',
			name: 'Matthew Ehlen',
			position: 'Owner & Co-Founder',
			description:
				'Matthew is the head of our Asheville, NC branch, overseeing all operations and helping our clients Dominate Their Market.',
			facebook: 'https://www.facebook.com/matthew.ehlen.96',
			linkedin: 'https://www.linkedin.com/in/matthew-ehlen-291926104/'
		},
		{
			image: '../static/images/team/brian-robinson.jpg',
			name: 'Brian Robinson',
			position: 'Chief Operating Officer',
			description:
				'Brian is responsible for the day-to-day operations of the agency as a whole, along with many other duties and responsibilities.',
			facebook: 'https://www.facebook.com/profile.php?id=100012837815683',
			linkedin: 'https://www.linkedin.com/in/brian-robinson-613312195/'
		},
		{
			image: '../static/images/team/gregory-troche.jpg',
			name: 'Gregory Troche',
			position: 'Web & PPC Manager',
			description:
				'Greg oversees every Website Design and Development project and manages Pay Per Click campaigns on Google and Facebook.',
			facebook: 'https://www.facebook.com/profile.php?id=100070422854240',
			linkedin: 'https://www.linkedin.com/in/gregorytroche/'
		},
		{
			image: '../static/images/team/rawan-walters.jpg',
			name: 'Rawan Walters',
			position: 'Sales Manager',
			description:
				'Rawan manages the Admin team, overseeing our Help Desk which answers all client requests, inquiries, and onboarding procedures.',
			facebook: 'https://www.facebook.com/rawan.walters',
			linkedin: ''
		},
		{
			image: '../static/images/team/nichole-gallo.jpg',
			name: 'Nichole Gallo',
			position: 'Seo Specialist',
			description:
				'Nicole helps our clients thrive in a competitive market by implementing SEO strategies to improve search engine ranking and increase site traffic.',
			facebook: '',
			linkedin: ''
		}
	];

	//# Get even and odds from the teamMembers array
	// let teamMemberOdd = teamMember.filter((element, index) => {
	// 	return index % 2 === 0;
	// });

	// let teamMemberEven = teamMember.filter((element, index) => {
	// 	return index % 2 !== 0;
	// });
</script>

<script>
	// import Carousel from 'svelte-carousel';
	import Heading from '$lib/components/Heading.svelte';
	import { onMount } from 'svelte';

	let heading = 'Our Team';
	let subHeading =
		'Unlike most digital marketing agencies, all of our employees work in-house. In our office, collaboration and communication are a key focus every single day.';
	let align = 'center';

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
		let:loaded
		autoplay
		autoplayDuration={5000}
		particlesToShow={2}
		particlesToScroll={2}
		arrows={false}
		dots={false}
	>
		{#each teamMember as team}
			<div class="wrap">
				<div class="team-member">
					<img src={team.image} alt={team.name} />
					<div class="info">
						<h3 class="title">{team.name}</h3>
						<p class="position">{team.position}</p>
						<p class="description">{team.description}</p>
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
		color: var(--color-white);
		padding: 5rem 0;
	}

	/* display two */
	.wrap {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		align-items: center;
		margin-bottom: 10rem;
	}
	.team-member {
		display: flex;
		flex-direction: row;
		align-items: top;
		width: 35%;
		height: 30rem;
		background-color: var(--color-white);
		color: var(--color-black);
		box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.1);
	}

	.info {
		padding: 2rem;
	}

	.title {
		font-size: 2rem;
		font-weight: bold;
		margin-bottom: 0.5rem;
	}

	.position {
		font-size: 1.3rem;
		font-weight: bold;
		margin-bottom: 1rem;
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
		font-size: 2rem;
		color: var(--color-black);
	}
</style>
