<script>
	import gradient1 from '$lib/images/gradient-1.webp';
	import gradient1_fallback from '$lib/images/gradient-1.png';
</script>

<section>
	<div class="container">
		<h2>
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
		padding-left: 10px;
		animation: spin-words 10s infinite;
	}

	.words {
		overflow: hidden;
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
		font-size: 2.5rem;
		font-weight: 700;
		color: var(--color-white-0);
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
</style>
