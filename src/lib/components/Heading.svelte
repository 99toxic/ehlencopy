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
		margin: 4rem auto;
	}

	.left hr {
		margin: 2rem 0;
	}
</style>
