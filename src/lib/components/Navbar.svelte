<script lang="ts">
	import MediaQuery from './MediaQuery.svelte';
	import { fly } from 'svelte/transition';
	import AnimatedHamburger from './AnimatedHamburger.svelte';
	import ActiveLink from '$lib/components/ActiveLink.svelte';

	export let open = false;
	export let onClick = () => {
		open = !open;
	};
</script>

<div class="navbar">
	<!-- <div class="logo">
		<a href="index.html">
			<img src="../images/logo.png" alt="logo" />
		</a>
	</div> -->
	<div class="menu">
		<MediaQuery query="(min-width: 1281px)" let:matches>
			{#if matches}
				<nav>
					<ul>
						<li><ActiveLink class="home" href="/">Home</ActiveLink></li>
						<li><ActiveLink href="/about">About</ActiveLink></li>
						<li><ActiveLink href="/services">Services</ActiveLink></li>
						<li><ActiveLink href="/support-forms">Support Forms</ActiveLink></li>
						<li><ActiveLink href="/contact">Contact Us</ActiveLink></li>
					</ul>
				</nav>
			{/if}
		</MediaQuery>

		<MediaQuery query="(max-width: 1280px)" let:matches>
			{#if matches}
				<AnimatedHamburger {open} {onClick} />
			{/if}
		</MediaQuery>
	</div>
</div>

{#if open}
	<nav class="mobile-nav" transition:fly={{ y: -200, duration: 400 }}>
		<ul>
			<li><ActiveLink class="home" href="/">Home</ActiveLink></li>
			<li><ActiveLink href="/about">About</ActiveLink></li>
			<li><ActiveLink href="/services">Services</ActiveLink></li>
			<li><ActiveLink href="/support-forms">Support Forms</ActiveLink></li>
			<li><ActiveLink href="/contact">Contact Us</ActiveLink></li>
		</ul>
	</nav>
{/if}

<style>
	.navbar {
		display: flex;
		justify-content: flex-end;
		padding: 2rem 5rem;
	}

	.menu nav ul {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	.menu nav ul li {
		display: flex;
		align-items: center;
		justify-content: center;
		margin-right: 1rem;
	}

	.mobile-nav {
		position: absolute;
		z-index: 2;
		width: 100vw;
		padding: 1rem;
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
		align-items: center;
		background-color: var(--color-black);
	}

	.mobile-nav ul {
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
		align-items: center;
		list-style-type: none;
	}
	.mobile-nav ul li a {
		font-size: 5rem;
		color: var(--color-tertiary);
		text-decoration: none;
		text-transform: uppercase;
		font-weight: bold;
	}

	/* //# Add active class to navigation when on page */
	/* .active {
		color: var(--color-secondary);
	} */
</style>
