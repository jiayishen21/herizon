<script>
</script>

<section>
	<h2>Stay tuned for what's around the corner.</h2>

	<div class="events-grid">
		<div class="picture-container">
			<picture>
				<!-- <source srcset={michelle_zatlyn} type="image/webp" /> -->
				<img
					src="https://www.koimoi.com/wp-content/new-galleries/2020/12/bryan-cranston-aka-walter-white-thinks-making-a-breaking-bad-movie-isnt-a-good-idea001.jpg"
					alt="walter white"
				/>
			</picture>

			<div class="desc">
				<p>Walter H. White,</p>
				<p>Drug Chemist</p>
				<p class="details">Sep. 11, 2023</p>
			</div>
		</div>

		<div class="picture-container">
			<picture>
				<!-- <source srcset={michelle_zatlyn} type="image/webp" /> -->
				<img
					src="https://media.npr.org/assets/img/2019/10/11/gb_00600r_wide-4de5e65a4a8f45e7d925d0e7999a3767c4eff9e4.jpg"
					alt="jessie pinkman"
				/>
			</picture>

			<div class="desc">
				<p>Jessie Pinkman,</p>
				<p>Drug Distributor</p>
				<p class="details">Sep. 11, 2023</p>
			</div>
		</div>
	</div>
</section>

<style>
	section {
		margin-top: 6rem;
	}

	h2 {
		font-size: 3rem;
		font-weight: 700;
		text-align: center;
	}

	.events-grid {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1.5rem;
		margin: 1.8rem 0;
	}

	.picture-container {
		position: relative;
		height: 400px;
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
		position: absolute;
		bottom: 0;
		left: 0;
		border-radius: 10px;
		padding: 1.3rem 3rem;
		background: rgba(255, 255, 255, 0.25);
		width: 100%;
		backdrop-filter: blur(20px);
		color: var(--color-white-0);
		font-size: 1.7rem;
		font-weight: 700;
	}

	.picture-container .details {
		margin-top: 0.5rem;
		font-size: 1.2rem;
		font-weight: 400;
		font-family: var(--font-mono);
	}

	@media (max-width: 1300px) {
		.picture-container .desc {
			font-size: 1.4rem;
		}

		.picture-container .details {
			font-size: 1.4rem;
		}
	}

	@media (max-width: 1100px) {
		.picture-container img {
			height: 450px;
		}

		.picture-container .desc {
			font-size: 1.3rem;
		}

		.picture-container .details {
			font-size: 1.3rem;
		}
	}

	@media (max-width: 950px) {
		h2 {
			font-size: 3rem;
			flex-direction: row;
			height: 80px;
		}

		.words {
			height: 100px;
			padding-left: 10px;
		}

		.container p {
			font-size: 1.2rem;
		}

		.container a {
			margin-top: 1.5rem;
			font-size: 1.2rem;
		}

		.join-us-banner img {
			height: 250px;
		}

		.join-us a {
			display: none;
		}

		section {
			display: flex;
			flex-direction: column-reverse;
		}

		.banner-heading {
			display: flex;
			position: absolute;
			bottom: 2rem;
			left: 3rem;
			color: var(--color-white-0);
		}

		.container-heading {
			display: none;
		}

		.desc {
			margin-top: 2rem;
		}
	}

	@media (max-width: 800px) {
		.banner-heading {
			flex-direction: column;
			height: 130px;
		}

		.words {
			height: 80px;
			padding-left: 0;
		}

		.desc {
			padding: 0;
		}
	}

	@media (max-width: 500px) {
		.banner-heading {
			font-size: 2rem;
			height: 100px;
			bottom: 1rem;
		}

		.words {
			height: 60px;
		}

		.join-us-banner img {
			height: 180px;
		}
	}
</style>
