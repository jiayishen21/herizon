<script>
	import Navbar from './Navbar.svelte';
	import '../app.css';
	import Footer from './Footer.svelte';
</script>

<div class="app">
	<Navbar />

	<main>
		<slot />
	</main>

	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		box-sizing: border-box;
		width: 100%;
		padding: 0 5rem;
		max-width: 1300px;
		margin: 0 auto;
	}

	@media (max-width: 768px) {
		main {
			padding: 0 2rem;
		}
	}

	@media (max-width: 500px) {
		main {
			padding: 0 1rem;
		}
	}
</style>
