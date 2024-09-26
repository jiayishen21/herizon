<script>
	import michelle_zatlyn from '$lib/images/michelle-zatlyn.webp';
	import michelle_zatlyn_fallback from '$lib/images/michelle-zatlyn.png';
</script>

<section>
	<h2>Inspiration from around the world.</h2>

	<div class="news-grid">
		<div class="picture-container tall-block">
			<picture>
				<source srcset={michelle_zatlyn} type="image/webp" />
				<img src={michelle_zatlyn_fallback} alt="michelle zatlyn" />
			</picture>

			<div class="desc">
				<p>Michelle Zatlyn,</p>
				<p>COO at CloudFlare</p>
			</div>
		</div>

		<div class="picture-container wide-block wide-block-0">
			<picture>
				<source srcset={michelle_zatlyn} type="image/webp" />
				<img src={michelle_zatlyn_fallback} alt="michelle zatlyn" />
			</picture>
		</div>
		<div class="picture-container wide-block wide-block-1">
			<picture>
				<source srcset={michelle_zatlyn} type="image/webp" />
				<img src={michelle_zatlyn_fallback} alt="michelle zatlyn" />
			</picture>
		</div>
	</div>
</section>

<style>
	section {
		margin-top: 2.5rem;
	}

	h2 {
		font-size: 2.5rem;
		font-weight: 700;
		text-align: center;
	}

	.news-grid {
		display: grid;
		grid-template-columns: 8fr 7fr 7fr;
		grid-template-rows: auto;
		gap: 1.5rem;
		height: 600px;
		margin: 1.8rem 0;
	}

	.picture-container {
		position: relative;
	}

	.tall-block {
		grid-row: 1 / span 2;
		grid-column: 1;
		height: 600px;
	}

	.wide-block {
		height: calc(300px - 0.75rem);
		grid-column: 2 / span 2;
	}

	.wide-block-0 {
		grid-row: 1;
	}

	.wide-block-1 {
		grid-row: 2;
	}

	picture {
		width: 100%;
		height: 100%;
		display: block;
	}

	picture img {
		display: flex;
		width: 100%;
		height: 100%;
		object-fit: cover;
		object-position: center;
		border-radius: 10px;
	}

	.picture-container .desc {
		text-align: end;
		position: absolute;
		bottom: 1rem;
		right: 1rem;
		color: var(--color-white-0);
		font-size: 1.7rem;
		font-weight: 700;
		filter: drop-shadow(0 1px 4px var(--color-shadow-0));
	}
</style>
