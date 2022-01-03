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
		}
	];
</script>

<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Our Team';
	let subHeading =
		'Unlike most digital marketing agencies, all of our employees work in-house. In our office, collaboration and communication are a key focus every single day.';
	let align = 'center';
</script>

<section>
	<Heading {heading} {subHeading} {align} />
	<div class="wrap">
		{#each teamMember as team}
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
		{/each}
	</div>
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
		align-items: flex-start;
		margin: 0;
	}
	.team-member {
		margin: 10rem 2rem;
		display: flex;
		flex-direction: row;
		align-items: top;
		justify-content: space-between;
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
