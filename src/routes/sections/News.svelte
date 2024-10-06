<script>
	import michelle_zatlyn from '$lib/images/michelle-zatlyn.webp';
	import michelle_zatlyn_fallback from '$lib/images/michelle-zatlyn.png';
	import emily_weiss from '$lib/images/emily-weiss.webp';
	import emily_weiss_fallback from '$lib/images/emily-weiss.png';
	import sarah_blakely from '$lib/images/sarah-blakely.webp';
	import sarah_blakely_fallback from '$lib/images/sarah-blakely.png';
</script>

<section>
	<h2>Inspiration from around the world.</h2>

	<div class="news-grid">
		<a
			href="https://www.elle.com/beauty/a60112997/emily-weiss-women-of-impact-interview-2024/"
			class="picture-container wide-block wide-block-0"
			target="_blank"
		>
			<picture>
				<source srcset={emily_weiss} type="image/webp" />
				<img src={emily_weiss_fallback} alt="emily weiss" />
			</picture>

			<div class="desc">
				<p>Emily Weiss,</p>
				<p>CEO of Glossier</p>
			</div>
		</a>

		<a href="https://youtu.be/2NgyaeCku_8" class="picture-container tall-block" target="_blank">
			<picture>
				<source srcset={michelle_zatlyn} type="image/webp" />
				<img src={michelle_zatlyn_fallback} alt="michelle zatlyn" />
			</picture>

			<div class="desc">
				<p>Michelle Zatlyn,</p>
				<p>COO of CloudFlare</p>
			</div>
		</a>

		<a
			href="https://www.masterclass.com/articles/sara-blakely-founder-of-spanx"
			class="picture-container wide-block wide-block-1"
			target="_blank"
		>
			<picture>
				<source srcset={sarah_blakely} type="image/webp" />
				<img src={sarah_blakely_fallback} alt="sarah blakely" />
			</picture>

			<div class="desc">
				<p>Sarah Blakely,</p>
				<p>Founder of Spanx</p>
			</div>
		</a>
	</div>
</section>

<style>
	section {
		margin-top: 3rem;
	}

	h2 {
		font-size: 3rem;
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
		border-radius: 10px;
		overflow: hidden;
		display: block;
	}

	picture img {
		display: flex;
		width: 100%;
		height: 100%;
		object-fit: cover;
		object-position: top;
		border-radius: 10px;
		transition: transform 0.5s ease;
	}

	picture img:hover {
		transform: scale(1.1);
	}

	.picture-container .desc {
		text-align: end;
		position: absolute;
		bottom: 1rem;
		color: var(--color-white-0);
		font-size: 1.7rem;
		font-weight: 700;
		filter: drop-shadow(0 1px 3px var(--color-shadow-1));
		right: 1rem;
	}

	@media (max-width: 1300px) {
		.news-grid {
			grid-template-columns: 8fr 6fr 6fr;
			height: 500px;
		}

		h2 {
			font-size: 2.5rem;
		}

		.picture-container .desc {
			font-size: 1.5rem;
		}

		.tall-block {
			height: 500px;
		}

		.wide-block {
			height: calc(250px - 0.75rem);
		}
	}

	@media (max-width: 950px) {
		.news-grid {
			height: 400px;
		}

		h2 {
			font-size: 2rem;
		}

		.picture-container .desc {
			font-size: 1.3rem;
		}

		.tall-block {
			height: 400px;
		}

		.wide-block {
			height: calc(200px - 0.75rem);
		}
	}

	@media (max-width: 768px) {
		h2 {
			font-size: 1.75rem;
		}

		.picture-container .desc {
			font-size: 1.2rem;
		}

		.news-grid {
			display: flex;
			flex-direction: column;
			max-width: 400px;
			margin: 0 auto;
			margin-top: 1.5rem;
			height: fit-content;
		}

		.tall-block {
			height: 500px;
		}

		.wide-block {
			grid-row: 1;
			grid-column: 1;
			height: 250px;
		}
	}

	@media (max-width: 450px) {
		.tall-block {
			height: auto;
		}

		.wide-block {
			height: auto;
		}
	}
</style>
