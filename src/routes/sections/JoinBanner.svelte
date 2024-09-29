<script>
	import gradient2 from '$lib/images/gradient-2.webp';
	import gradient2_fallback from '$lib/images/gradient-2.png';
	import chevron from '$lib/images/chevron.svg';
</script>

<section>
	<div class="hero-container">
		<picture class="hero">
			<source srcset={gradient2} type="image/webp" />
			<img src={gradient2_fallback} alt="herizon hero" />
		</picture>

		<h2>Join our community of entrepreneurs.</h2>

		<a href="youtube.com">Membership applications here</a>

		<div class="learn-more">
			<p>Learn more</p>
			<img src={chevron} alt="chevron" />
		</div>
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

	.hero-container h2 {
		max-width: 850px;
		position: absolute;
		top: 7rem;
		left: 12rem;
		font-size: 3rem;
		font-weight: 700;
		filter: drop-shadow(0 1px 4px var(--color-shadow-0));
	}

	.hero-container a {
		position: absolute;
		top: 19rem;
		left: 16rem;
		font-size: 1.6rem;
		filter: drop-shadow(0 1px 2px var(--color-shadow-0));
		text-decoration: underline;
		color: var(--color-white-0);
	}

	.learn-more {
		position: absolute;
		bottom: 4.5rem;
		left: 50%;
		transform: translate(-50%, 0);
		font-size: 1.6rem;
		filter: drop-shadow(0 1px 2px var(--color-shadow-0));
		color: var(--color-white-0);
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.learn-more img {
		margin-top: 0.5rem;
		width: 70%;
		height: auto;
	}
</style>
