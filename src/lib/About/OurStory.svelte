<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = `Our Story`;
	let subHeading = ``;
	let align = `center`;
</script>

<section>
	<Heading {heading} {subHeading} {align} />

	<div class="year-1">
		<h3>2017</h3>
		<p>Ehlen Analytics was founded by brothers Daniel and Mathew Ehlen in Asheville, NC</p>
	</div>

	<div class="year-2">
		<h3>2018</h3>
		<p>We moved into our first office, our first stepping stone of measurable success</p>
	</div>

	<div class="year-3">
		<h3>2019</h3>
		<p>We were nominated as one of the Premier Digital Marketing Agencies in the United States</p>
	</div>

	<div class="year-4">
		<h3>2020</h3>
		<p>
			We experienced tremendous growth during the height of COVID, and began to steadily expand our
			fulfillment team
		</p>
	</div>

	<div class="year-5">
		<h3>2021</h3>
		<p>
			We established our second branch in Bradenton, FL to expand our reach and continue growing our
			team
		</p>
	</div>
</section>

<style lang="scss">
	section {
		width: 40%;
		margin: 0 auto;

		.year-1 {
			background-color: var(--color-tertiary);
			padding: 1rem;
			margin: 1rem;
			text-align: center;
			position: relative;

			::before {
				content: '';
				display: block;
				width: 0;
				height: 0;
				border-top: 12px solid transparent;
				border-bottom: 12px solid transparent;
				border-left: 12px solid var(--color-tertiary);
				position: absolute;
				top: 16px;
				right: -12px;
			}
		}

		.year-2 {
			background-color: var(--color-tertiary);
			padding: 1rem;
			margin: 1rem;

			h3 {
				text-align: center;
			}

			p {
				text-align: right;
			}

			::before {
				content: '';
				display: block;
				width: 0;
				height: 0;
				border-top: 12px solid transparent;
				border-bottom: 12px solid transparent;
				border-left: 12px solid var(--color-tertiary);
				position: absolute;
				top: 16px;
				right: -12px;
			}
		}

		.year-3 {
			background-color: var(--color-tertiary);
			padding: 1rem;
			margin: 1rem;

			h3 {
				text-align: center;
			}

			::before {
				content: '';
				display: block;
				width: 0;
				height: 0;
				border-top: 12px solid transparent;
				border-bottom: 12px solid transparent;
				border-left: 12px solid var(--color-tertiary);
				position: absolute;
				top: 16px;
				right: -12px;
			}
		}

		.year-4 {
			background-color: var(--color-tertiary);
			padding: 1rem;
			margin: 1rem;

			h3 {
				text-align: center;
			}

			p {
				text-align: right;
			}

			::before {
				content: '';
				display: block;
				width: 0;
				height: 0;
				border-top: 12px solid transparent;
				border-bottom: 12px solid transparent;
				border-left: 12px solid var(--color-tertiary);
				position: absolute;
				top: 16px;
				right: -12px;
			}
		}

		.year-5 {
			background-color: var(--color-tertiary);
			padding: 1rem;
			margin: 1rem;

			h3 {
				text-align: center;
			}

			::before {
				content: '';
				display: block;
				width: 0;
				height: 0;
				border-top: 12px solid transparent;
				border-bottom: 12px solid transparent;
				border-left: 12px solid var(--color-tertiary);
				position: absolute;
				top: 16px;
				right: -12px;
			}
		}
	}
</style>
