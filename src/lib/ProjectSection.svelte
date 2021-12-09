<script>
	import Heading from './Heading.svelte';
	let heading = 'Our Projects';
	let subHeading = 'Expertly designed and fully optimized websites.';
</script>

<div class="projects">
	<Heading {heading} {subHeading} />
	<div class="projects__wrap">
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/engergyn-website-design.jpg" alt="Energyn" />
			</div>
			<div class="projects__item__text">
				<h3>Energyn</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/jwrestores-website-design.jpg" alt="JW Restores" />
			</div>
			<div class="projects__item__text">
				<h3>JW Restores</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/bluelineelectric-website-design.jpg" alt="Blue Line Electric" />
			</div>
			<div class="projects__item__text">
				<h3>Blue Line Electric</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img
					src="images/projects/jadespremiumqualitycleaning-website-design.jpg"
					alt="Jades Premium quality Cleaning"
				/>
			</div>
			<div class="projects__item__text">
				<h3>Jades Premium quality Cleaning</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img
					src="images/projects/ridgeappliancerepair-website-design.jpg"
					alt="Ridge Appliance Repair"
				/>
			</div>
			<div class="projects__item__text">
				<h3>Ridge Appliance Repair</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/totalroofingofatl-website-design.jpg" alt="Total Roofing ATL" />
			</div>
			<div class="projects__item__text">
				<h3>Total Roofing ATL</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/arhthomesolutions-website-design.jpg" alt="Blue Line Electric" />
			</div>
			<div class="projects__item__text">
				<h3>Blue Line Electric</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/imperialchemdry-website-design.jpg" alt="Imperial Chem Dry" />
			</div>
			<div class="projects__item__text">
				<h3>Imperial Chem dry</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
		<div class="projects__item">
			<div class="projects__item__image">
				<img src="images/projects/hammondhill-website-design.jpg" alt="Hammond Hill" />
			</div>
			<div class="projects__item__text">
				<h3>Hammond Hill</h3>
				<p>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec euismod, tortor eu
					consectetur congue, nisi nisl aliquet nisl, eget consectetur nunc nisl euismod nunc.
				</p>
				<a href="/">Read More</a>
			</div>
		</div>
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
	.projects__wrap {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		grid-gap: 4rem;
		margin-top: 5rem;
	}
	.projects__item {
		width: 100%;
	}
	.projects__item__image img {
		width: 100%;
	}
</style>
