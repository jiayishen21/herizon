<script>
	import Events from './sections/Events.svelte';
	import Faq from './sections/Faq.svelte';
	import Hero from './sections/Hero.svelte';
	import Mission from './sections/Mission.svelte';
	import News from './sections/News.svelte';
	import Partner from './sections/Partner.svelte';
</script>

<svelte:head>
	<title>herizon</title>
	<meta
		name="description"
		content="herizon supports female entrepreneurs in creating small businesses, researching their market, and connecting with industry professionals."
	/>
</svelte:head>

<Hero />
<News />
<Mission />
<Partner />
<!-- <Events /> -->
<Faq />
