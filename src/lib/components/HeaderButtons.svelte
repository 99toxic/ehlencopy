<script>
	import ButtonOne from '$lib/components/ButtonOne.svelte';
	import ButtonTwo from '$lib/components/ButtonTwo.svelte';
</script>

<div class="header-buttons">
	<ButtonOne />
	<ButtonTwo />
</div>

<style>
	.header-buttons {
		align-items: center;
		display: flex;
		justify-content: space-evenly;
		margin: 0 auto;
		width: 40%;
	}

	.header-buttons__contact {
		border-radius: 5rem;
		color: var(--color-tertiary);
		font-size: 2rem;
		font-weight: 700;
		margin-top: 1.5rem;
		padding: 2rem 3.5rem;
		text-decoration: none;
		text-transform: uppercase;
	}

	.header-buttons__contact {
		background: var(--color-gradient-primary);
	}

	.header-buttons__contact:hover {
		background: var(--color-secondary);
	}
</style>
