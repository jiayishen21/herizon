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
			Partnering with <br />
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
		font-size: 2.5rem;
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
</style>
