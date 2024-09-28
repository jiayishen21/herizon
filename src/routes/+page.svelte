<script>
	import Events from './sections/Events.svelte';
	import Faq from './sections/Faq.svelte';
	import Hero from './sections/Hero.svelte';
	import Mission from './sections/Mission.svelte';
	import News from './sections/News.svelte';
	import Partner from './sections/Partner.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<Hero />
<News />
<Mission />
<Partner />
<Events />
<Faq />
