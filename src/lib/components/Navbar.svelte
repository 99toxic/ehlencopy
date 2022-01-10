<script lang="ts">
	import MediaQuery from '$lib/components/MediaQuery.svelte';
	import { fly } from 'svelte/transition';
	import AnimatedHamburger from '$lib/components/AnimatedHamburger.svelte';
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
		<MediaQuery query="(min-width: 1100px)" let:matches>
			{#if matches}
				<nav>
					<ul>
						<li><ActiveLink class="home" href="/">Home</ActiveLink></li>
						<li><ActiveLink href="/about">About</ActiveLink></li>
						<li><ActiveLink href="/services">Services</ActiveLink></li>
						<li><ActiveLink href="/support-forms">Support Forms</ActiveLink></li>
						<li><ActiveLink href="/blog">Blog</ActiveLink></li>
						<li><ActiveLink href="/contact">Contact Us</ActiveLink></li>
					</ul>
				</nav>
			{:else}
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
			<li><ActiveLink href="/blog">Blog</ActiveLink></li>
			<li><ActiveLink href="/contact">Contact Us</ActiveLink></li>
		</ul>
	</nav>
{/if}

<style>
	.navbar {
		display: flex;
		justify-content: flex-end;
	}

	.menu nav ul {
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 2rem 5rem;
	}

	.menu nav ul li {
		display: flex;
		align-items: center;
		justify-content: center;
		margin-right: 2rem;
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
</style>
