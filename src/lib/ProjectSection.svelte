<script>
	import Heading from './Heading.svelte';
	import { projects } from '../stores/projectImages';
	let heading = 'Our Projects';
	let subHeading = 'Expertly designed and fully optimized websites.';
</script>

<div class="projects">
	<Heading {heading} {subHeading} />
	<div class="wrap">
		{#each projects as project}
			<div class="item">
				<div class="image">
					<img src={project.image} alt={project.title} />
				</div>
				<!-- //# Will add this later (part of projectImages)-->
				<!-- <div class="text">
					<h3>{project.title}</h3>
					<p>
						{project.description}
					</p>
					<a href="/">Read More</a>
				</div> -->
			</div>
		{/each}
	</div>
</div>

<style>
	.projects {
		background: url('../images/main-projects-bg.png') no-repeat right top;
		background-size: fit;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		padding: 20rem;
	}
	.wrap {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		grid-gap: 4rem;
		margin-top: 5rem;
	}
	.item {
		width: 100%;
	}
	.image img {
		width: 100%;
	}
</style>
