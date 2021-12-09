<script lang="ts">
	import HomeHeader from '$lib/HomeHeader.svelte';
	import HomeHeaderCTA from '$lib/HomeHeaderCTA.svelte';
	import Heading from '$lib/Heading.svelte';
	import ServicesSection from '$lib/ServicesSection.svelte';
	import CTAOne from '$lib/CTAOne.svelte';
	import ProjectsSection from '$lib/ProjectsSection.svelte';
	import WhyUsSection from '$lib/WhyUsSection.svelte';

	let heading = 'Our digital marketing services';
	let subHeading =
		'Our services are uniquely optimized for each individual client, to best suit your needs.';

	let title = 'Digital Marketing Agency';
</script>

<svelte:head>
	<title>{title} | Ehlen Analytics</title>
</svelte:head>

<HomeHeader />
<HomeHeaderCTA />
<Heading {heading} {subHeading} />
<ServicesSection />
<CTAOne />
<ProjectsSection />
<WhyUsSection />
