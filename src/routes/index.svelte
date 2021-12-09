<script lang="ts">
	import HomeHeader from '$lib/HomeHeader.svelte';
	import HomeHeaderCTA from '$lib/HomeHeaderCTA.svelte';
	import Heading from '$lib/Heading.svelte';
	import ServicesSection from '$lib/ServicesSection.svelte';
	import CTAOne from '$lib/CTAOne.svelte';
	import ProjectSection from '$lib/ProjectSection.svelte';
	import WhyUsSection from '$lib/WhyUsSection.svelte';

	let heading = 'Our digital marketing services';
	let subHeading =
		'Our services are uniquely optimized for each individual client, to best suit your needs.';

	let title = 'Digital Marketing Agency';
</script>

<svelte:head>
	<!-- Google Fonts -->
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Raleway&display=swap"
		rel="stylesheet"
	/>

	<!-- Font-Awesome -->
	<link
		rel="stylesheet"
		href="https://use.fontawesome.com/releases/v5.0.13/css/all.css"
		integrity="sha384-DNOHZ68U8hZfKXOrtjWvjxusGo9WQnrNx2sqG0tfsghAvtVlRW3tvkXWZh58N9jp"
		crossorigin="anonymous"
	/>

	<title>{title} | Ehlen Analytics</title>
</svelte:head>

<HomeHeader />
<HomeHeaderCTA />
<Heading {heading} {subHeading} />
<ServicesSection />
<CTAOne />
<ProjectSection />
<WhyUsSection />
