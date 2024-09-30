<script>
	import gradient1 from '$lib/images/gradient-1.webp';
	import gradient1_fallback from '$lib/images/gradient-1.png';
</script>

<section>
	<div class="container">
		<h2 class="container-heading">
			Becoming
			<div class="words">
				<span>great.</span>
				<span>tenatious.</span>
				<span>curious.</span>
				<span>resourceful.</span>
				<span>hungry.</span>
			</div>
		</h2>

		<p class="desc">
			Supporting young women to become entrepreneurs. We also provide opportunities to chat,
			network, and consult with industry experts. Join us for free for the first three months of our
			launch to meet seasoned professionals in tech, fashion, and beauty.
		</p>

		<a href="/join">Learn more</a>
	</div>

	<div class="join-us">
		<picture class="join-us-banner">
			<source srcset={gradient1} type="image/webp" />
			<img src={gradient1_fallback} alt="join herizon" />
		</picture>
		<a href="/join">Join today</a>
		<h2 class="banner-heading">
			Becoming
			<div class="words">
				<span>great.</span>
				<span>tenatious.</span>
				<span>curious.</span>
				<span>resourceful.</span>
				<span>hungry.</span>
			</div>
		</h2>
	</div>
</section>

<style>
	section {
		margin-top: 3.5rem;
		display: grid;
		grid-template-columns: 14fr 8fr;
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

	.container a {
		margin-top: 3rem;
		font-size: 1.5rem;
		font-family: var(--font-mono);

		color: var(--color-black-0);
	}

	h2 {
		box-sizing: content-box;
		height: 90px;
		display: flex;
		font-size: 3.2rem;
		font-weight: 700;
	}

	.desc {
		padding-right: 2rem;
		line-height: 1.3;
	}

	.words span {
		display: block;
		height: 100%;
		animation: spin-words 10s infinite;
	}

	.words {
		overflow: hidden;
		padding-left: 10px;
	}

	.join-us-banner {
		width: 100%;
		display: block;
	}

	.join-us-banner img {
		width: 100%;
		height: 600px;
		object-fit: cover;
		border-radius: 10px;
	}

	.join-us {
		position: relative;
	}

	.join-us a {
		position: absolute;
		bottom: 3rem;
		left: 50%;
		transform: translate(-50%, 0);
		font-size: 3rem;
		width: 100%;
		text-align: center;
		font-weight: 700;
		color: var(--color-white-0);
	}

	.banner-heading {
		display: none;
	}

	@keyframes spin-words {
		0% {
			transform: translateY(-12%);
		}
		13% {
			transform: translateY(0);
		}
		19% {
			transform: translateY(-112%);
		}
		32% {
			transform: translateY(-100%);
		}
		38% {
			transform: translateY(-212%);
		}
		51% {
			transform: translateY(-200%);
		}
		57% {
			transform: translateY(-312%);
		}
		70% {
			transform: translateY(-300%);
		}
		76% {
			transform: translateY(-412%);
		}
		89% {
			transform: translateY(-400%);
		}
		100% {
			transform: translateY(-12%);
		}
	}

	@media (max-width: 1300px) {
		section {
			grid-template-columns: 14fr 8fr;
		}

		.container {
			padding-left: 2rem;
			padding-right: 4rem;
		}

		.container p {
			font-size: 1.4rem;
		}

		.container a {
			font-size: 1.4rem;
		}

		.join-us a {
			font-size: 2.5rem;
		}

		.join-us-banner img {
			height: 500px;
		}
	}

	@media (max-width: 1100px) {
		.join-us a {
			font-size: 2rem;
		}

		.join-us-banner img {
			height: 450px;
		}

		.container p {
			font-size: 1.3rem;
		}

		.container a {
			font-size: 1.3rem;
		}

		.container {
			padding-right: 2rem;
		}

		h2 {
			flex-direction: column;
			height: 150px;
		}

		.words {
			height: 80px;
			padding-left: 0;
		}
	}

	@media (max-width: 950px) {
		h2 {
			font-size: 2.9rem;
			flex-direction: row;
			height: 70px;
		}

		.words {
			height: 100%;
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
			left: 2.5rem;
			color: var(--color-white-0);
		}

		.container-heading {
			display: none;
		}

		.desc {
			margin-top: 2rem;
		}
	}

	@media (max-width: 768px) {
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

		.container {
			padding: 0 2rem;
		}

		.container p,
		.container a {
			font-size: 1.1rem;
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

		.container {
			padding: 0 1rem;
		}

		.container p,
		.container a {
			font-size: 1rem;
		}
	}
</style>
