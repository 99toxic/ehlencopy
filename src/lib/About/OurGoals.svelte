<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = `Our Goals`;
	let subHeading = `We’re here to offer you customized digital marketing solutions.`;
	let align = `center`;
</script>

<section>
	<Heading {heading} {subHeading} {align} />

	<div class="wrap">
		<div class="col">
			<i class="fab fa-google" />
			<p>
				First, we complete a deep analysis of your business using a deep-dive site audit tool during
				your free consultation
			</p>
		</div>
		<div class="col">
			<i class="fab fa-google" />
			<p>
				We help you create a customized marketing strategy that will maximize your potential by
				matching you up with the proper services for your needs
			</p>
		</div>
		<div class="col">
			<i class="fab fa-google" />
			<p>
				Our fulfillment team will conduct strategy sessions and begin the work necessary to create
				and optimize your online platforms
			</p>
		</div>
		<div class="col">
			<i class="fab fa-google" />
			<p>
				We will provide you with comprehensive reports on a monthly basis, that shows you steady
				development and measurable results
			</p>
		</div>
	</div>
</section>

<style lang="scss">
	section {
		background: url('/static/images/collage_for_dark.png') no-repeat bottom center;
		background-color: var(--color-black);
		background-size: fit;
		padding: 2rem 20rem 20rem;
		position: relative;
		z-index: 1;
		color: var(--color-white);

		.wrap {
			display: flex;
			flex-direction: row;
			justify-content: space-around;
			align-items: center;

			.col {
				display: flex;
				flex-direction: column;
				align-items: center;
				padding: 0 5rem;
				text-align: center;

				i {
					font-size: 5rem;
					color: var(--color-primary);
					margin-bottom: 2rem;
					background: var(--color-transparent-black);
					padding: 3rem;
				}
			}
		}
	}
</style>
