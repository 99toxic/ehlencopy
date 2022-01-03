<script>
	export let heading;
	export let subHeading;
	export let align;
</script>

<div class={align}>
	<h2>{heading}</h2>
	<hr />
	<p>{subHeading}</p>
</div>

<style>
	.center {
		padding: 5rem 0;
		text-align: center;
	}
	.left {
		width: 40%;
		text-align: left;
	}

	.center hr {
		width: 5rem;
		border: 2px solid var(--color-primary);
		margin: 2rem auto;
	}

	.left hr {
		width: 5rem;
		border: 2px solid var(--color-primary);
		margin: 2rem 0;
	}

	h2 {
		text-transform: uppercase;
	}

	p {
		margin-top: 2rem;
	}
</style>
