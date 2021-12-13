<script>
	export let heading;
	export let subHeading;
</script>

<div class="heading">
	<h2>{heading}</h2>
	<hr />
	<p>{subHeading}</p>
</div>

<style>
	.heading {
		background: url('../images/main-heading-bg.jpg') no-repeat;
		padding-top: 8rem;
		text-align: center;
	}

	h2 {
		text-transform: uppercase;
	}

	p {
		margin-top: 2rem;
	}
</style>
