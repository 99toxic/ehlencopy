<script context="module">
	export const projects = [
		{
			image: '../static/images/projects/arhthomesolutions-website-design.jpg',
			title: 'ARHT home Solutions',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/bluelineelectrictx-website-design.jpg',
			title: 'Blueline Electrictx',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/engergyn-website-design.jpg',
			title: 'Engergyn',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/hammondhill-website-design.jpg',
			title: 'Hammond Hill',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/imperialchemdry-website-design.jpg',
			title: 'Imperial Chem Dry',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/jadespremiumqualitycleaning-website-design.jpg',
			title: 'Jades Premium Quality Cleaning',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/jwrestores-website-design.jpg',
			title: 'JW Restores',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/laplumbingco-website-design.jpg',
			title: 'La Plumbing Co',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		},
		{
			image: '../static/images/projects/ridgeappliancerepair-website-design.jpg',
			title: 'Ridge Appliance Repair',
			description:
				'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		}
		//# One image too many (part of ProjectSection)
		// {
		// 	image: '../static/images/projects/totalroofingofatl-website-design.jpg',
		// 	title: 'Total Roofing of ATL',
		// 	description:
		// 		'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
		// }
	];
</script>

<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = 'Our Projects';
	let subHeading = 'Expertly designed and fully optimized websites.';
</script>

<section>
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
</section>

<style>
	section {
		background: url('../images/main-projects-bg.png') no-repeat right top;
		background-size: fit;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		padding: 0 20rem;
	}
	.wrap {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		grid-gap: 4rem;
	}
	.item {
		width: 100%;
	}
	.image img {
		width: 100%;
	}
</style>
