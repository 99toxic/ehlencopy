<script lang="ts">
	import HomeHeader from '$lib/home/HomeHeader.svelte';
	import ServicesSection from '$lib/home/ServicesSection.svelte';
	import CTAOne from '$lib/home/CTAOne.svelte';
	import ProjectSection from '$lib/home/ProjectSection.svelte';
	import WhyUsSection from '$lib/home/WhyUsSection.svelte';
	import TeamSection from '$lib/home/TeamSection.svelte';
	import CtaTwo from '$lib/home/CTATwo.svelte';
	import Testimonials from '$lib/home/Testimonials.svelte';
	import Badges from '$lib/home/Badges.svelte';
</script>

<svelte:head>
	<title>Digital Marketing Agency</title>
</svelte:head>

<HomeHeader />
<ServicesSection />
<CTAOne />
<ProjectSection />
<WhyUsSection />
<TeamSection />
<CtaTwo />
<Testimonials />
<Badges />
