<script>
	import backerfounder from '$lib/images/backer-founder.webp';
	import backerfounder_fallback from '$lib/images/backer-founder.png';
</script>

<section>
	<div>
		<picture class="sponsor-banner">
			<source srcset={backerfounder} type="image/webp" />
			<img src={backerfounder_fallback} alt="backer-founder" />
		</picture>
	</div>

	<div class="container">
		<h2>
			Partnering with<br class="break" />
			Backer-Founder.
		</h2>

		<p class="desc">
			We are working alongside Backer-Founder, Asia’s largest crowdfunding agency, providing equal
			opportunity to our members. We will support business owners meeting sufficient requirements in
			launching a crowdfunding campaign.
		</p>
	</div>
</section>

<style>
	section {
		margin-top: 3.5rem;
		display: grid;
		grid-template-columns: 8fr 14fr;
	}

	.container {
		display: flex;
		flex-direction: column;
		width: 100%;
		padding-left: 4rem;
		padding-right: 8rem;
		justify-content: center;
	}

	.container p {
		font-size: 1.5rem;
	}

	h2 {
		font-size: 3rem;
		font-weight: 700;
		margin-bottom: 1.8rem;
	}

	.desc {
		padding-right: 2rem;
		line-height: 1.3;
	}

	.sponsor-banner {
		width: 100%;
		display: block;
	}

	.sponsor-banner img {
		width: 100%;
		height: 600px;
		object-fit: cover;
		border-radius: 10px;
	}

	@media (max-width: 1300px) {
		section {
			grid-template-columns: 8fr 14fr;
		}

		.container {
			padding-left: 4rem;
			padding-right: 2rem;
		}

		h2 {
			font-size: 2.5rem;
		}

		.container p {
			font-size: 1.4rem;
		}

		.sponsor-banner img {
			height: 500px;
		}
	}

	@media (max-width: 1100px) {
		.sponsor-banner img {
			height: 450px;
		}

		.container p {
			font-size: 1.3rem;
		}

		.container {
			padding-left: 2rem;
		}
	}

	@media (max-width: 950px) {
		h2 {
			font-size: 2rem;
			margin-top: 1rem;
			margin-bottom: 0.5rem;
		}

		.container p {
			font-size: 1.2rem;
		}

		.sponsor-banner img {
			height: 250px;
		}

		section {
			display: flex;
			flex-direction: column;
		}

		.break {
			display: none;
		}
	}

	@media (max-width: 768px) {
		h2 {
			font-size: 1.75rem;
		}

		.container {
			padding: 0 2rem;
		}

		.sponsor-banner img {
			height: 180px;
		}

		.container p {
			font-size: 1.1rem;
		}

		.desc {
			padding: 0;
		}
	}

	@media (max-width: 500px) {
		.container {
			padding: 0 1rem;
		}

		.container p {
			font-size: 1rem;
		}
	}
</style>
