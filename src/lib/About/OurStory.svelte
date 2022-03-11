<script>
	import Heading from '$lib/components/Heading.svelte';
	let heading = `Our Story`;
	let subHeading = ``;
	let align = `center`;
</script>

<section>
	<Heading {heading} {subHeading} {align} />

	<div class="year year__1">
		<h3>2017</h3>
		<p>Ehlen Analytics was founded by brothers Daniel and Mathew Ehlen in Asheville, NC</p>
	</div>

	<div class="wrap">
		<div class="year year__2">
			<h3>2018</h3>
			<p>We moved into our first office, our first stepping stone of measurable success</p>
		</div>

		<div class="year year__3">
			<h3>2019</h3>
			<p>We were nominated as one of the Premier Digital Marketing Agencies in the United States</p>
		</div>

		<div class="year year__4">
			<h3>2020</h3>
			<p>
				We experienced tremendous growth during the height of COVID, and began to steadily expand
				our fulfillment team
			</p>
		</div>

		<div class="year year__5">
			<h3>2021</h3>
			<p>
				We established our second branch in Bradenton, FL to expand our reach and continue growing
				our team
			</p>
		</div>
	</div>
</section>

<style lang="scss">
	.wrap {
		background: linear-gradient(
			90deg,
			rgba(0, 0, 0, 0) calc(50% - 1px),
			var(--color-primary) calc(50%),
			rgba(0, 0, 0, 0) calc(50% + 1px)
		);
	}

	section {
		width: 40%;
		margin: 0 auto;

		.year {
			background-color: var(--color-tertiary);
			padding: 3rem;
			margin: 5rem;
			position: relative;

			&__1 {
				text-align: center;

				::before {
					content: '';
					position: absolute;
					bottom: 100%;
					left: 50%;
					transform: translateX(-50%);
					border: 11px solid transparent;
					border-bottom-color: var(--color-tertiary);
				}
			}

			&__2 {
				transform: translateX(-55%);

				h3 {
					text-align: center;
				}

				p {
					text-align: right;
				}

				::before {
					content: '';
					position: absolute;
					bottom: 50%;
					left: 100%;
					border: 11px solid transparent;
					border-left-color: var(--color-tertiary);
				}
			}

			&__3 {
				transform: translateX(55%);

				h3 {
					text-align: center;
				}

				::before {
					content: '';
					position: absolute;
					bottom: 50%;
					right: 100%;
					border: 11px solid transparent;
					border-right-color: var(--color-tertiary);
				}
			}

			&__4 {
				transform: translateX(-55%);

				h3 {
					text-align: center;
				}

				p {
					text-align: right;
				}

				::before {
					content: '';
					position: absolute;
					bottom: 50%;
					left: 100%;
					border: 11px solid transparent;
					border-left-color: var(--color-tertiary);
				}
			}

			&__5 {
				transform: translateX(55%);

				h3 {
					text-align: center;
				}

				::before {
					content: '';
					position: absolute;
					bottom: 50%;
					right: 100%;
					border: 11px solid transparent;
					border-right-color: var(--color-tertiary);
				}
			}
		}
	}
</style>
