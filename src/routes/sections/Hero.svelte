<script>
	import gradient0 from '$lib/images/gradient-0.webp';
	import gradient0_fallback from '$lib/images/gradient-0.png';
</script>

<section>
	<div class="hero-container">
		<picture class="hero">
			<source srcset={gradient0} type="image/webp" />
			<img src={gradient0_fallback} alt="herizon hero" />
		</picture>

		<h1>Becoming.</h1>

		<h4>Turning dreams into reality, one startup at a time.</h4>
	</div>
</section>

<style>
	.hero-container {
		margin: 3rem 0;
		position: relative;
		color: var(--color-white-0);
	}

	.hero {
		width: 100%;
		display: block;
	}

	.hero img {
		width: 100%;
		height: 600px;
		object-fit: cover;
		border-radius: 10px;
	}

	.hero-container h1 {
		position: absolute;
		top: 7rem;
		left: 50%;
		transform: translate(-50%, 0);
		font-size: 4.75rem;
		font-weight: 700;
		text-align: center;
		filter: drop-shadow(0 1px 4px var(--color-shadow-0));
	}

	.hero-container h4 {
		position: absolute;
		bottom: 5rem;
		left: 50%;
		transform: translate(-50%, 0);
		font-size: 2.2rem;
		font-family: var(--font-mono);
		font-weight: 400;
		text-align: center;
		filter: drop-shadow(0 1px 2px var(--color-shadow-0));
	}

	@media (max-width: 1300px) {
		.hero-container h1 {
			font-size: 3.5rem;
		}

		.hero-container h4 {
			font-size: 1.8rem;
			width: 100%;
			padding: 0 8rem;
		}
	}

	@media (max-width: 768px) {
		.hero-container h1 {
			font-size: 3rem;
		}

		.hero-container h4 {
			font-size: 1.5rem;
			width: 100%;
			padding: 0 2rem;
		}
	}

	@media (max-width: 600px) {
		.hero-container h1 {
			font-size: 2.5rem;
		}

		.hero-container h4 {
			font-size: 1.2rem;
			width: 100%;
			padding: 0 2rem;
		}
	}
</style>
