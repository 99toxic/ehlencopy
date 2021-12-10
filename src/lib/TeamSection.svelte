<script>
	import Heading from './Heading.svelte';
	import { teamMember } from '../stores/teamMembers';
	let heading = 'Our Team';
	let subHeading =
		'Unlike most digital marketing agencies, all of our employees work in-house. In our office, collaboration and communication are a key focus every single day.';
</script>

<div class="team">
	<Heading {heading} {subHeading} />
	<div class="wrap">
		{#each teamMember as team}
			<div class="team-member">
				<div class="team-member-image">
					<img src={team.image} alt={team.name} />
				</div>
				<div class="team-member-info">
					<h3>{team.name}</h3>
					<p>{team.position}</p>
					<p>{team.description}</p>
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
</div>

<style>
	.team {
		background: url('../images/team.jpg') no-repeat center top;
		background-size: fit;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-evenly;
		color: #fff;
		margin-top: 30rem;
	}
	.team-member {
		margin-top: 10rem;
		display: flex;
		flex-direction: row;
		align-items: top;
		justify-content: space-between;
	}
</style>
