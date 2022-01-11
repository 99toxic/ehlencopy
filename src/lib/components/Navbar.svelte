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
						<li>
							<ActiveLink href="/services">Services</ActiveLink>

							<!-- Dropdown menu for service pages -->
							<!-- <ul class="dropdown-menu" style="display: none;">
								<li><ActiveLink href="/local-national-seo">Local & National SEO</ActiveLink></li>
								<li>
									<ActiveLink href="/social-media-management">Social Media Management</ActiveLink>
								</li>
								<li><ActiveLink href="/content-writing">Content Writing</ActiveLink></li>
								<li>
									<ActiveLink href="/reputation-management">Reputation Management</ActiveLink>
								</li>
								<li>
									<ActiveLink href="/web-design-development">Web Design & Development</ActiveLink>
								</li>
								<li><ActiveLink href="/google-my-business">Google My Business</ActiveLink></li>
								<li><ActiveLink href="/google-ads">Google Ads</ActiveLink></li>
								<li><ActiveLink href="/facebook-ads">Facebook Ads</ActiveLink></li>
							</ul> -->
						</li>
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
