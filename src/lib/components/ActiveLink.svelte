<!-- ActiveLink credited to Evan Winter 'https://dev.to/evanwinter/active-links-in-sveltekit-4ihf' -->
<script>
	import { page } from '$app/stores';
	$: isActive = $page.path === $$props.href;
</script>

<a {...$$props} class:active={isActive}>
	<slot />
</a>

<style>
	a {
		font-size: 1.5rem;
		color: var(--color-tertiary);
		margin-right: 1rem;
		text-decoration: none;
		text-transform: uppercase;
		font-weight: bold;
	}

	a:hover {
		color: var(--color-primary);
	}

	a.active {
		color: var(--color-primary);
	}
</style>
