<script>
	import linkedin from '$lib/images/icons/linkedin.svg';
	import xiaohongshu from '$lib/images/icons/xiaohongshu.svg';
	import instagram from '$lib/images/icons/instagram.svg';
</script>

<footer>
	<div class="container">
		<p>@ 2024 herizon, all rights reserved</p>

		<ul>
			<li>
				<a href="https://www.linkedin.com/company/herizon-org/" target="_blank">
					<img src={linkedin} alt="linkedin" />
				</a>
			</li>
			<li>
				<a href="https://www.xiaohongshu.com/user/profile/66a1f3aa000000001d0336e5" target="_blank">
					<img src={xiaohongshu} alt="xiaohongshu" />
				</a>
			</li>
			<li>
				<a href="https://www.instagram.com/herizon.__/" target="_blank">
					<img src={instagram} alt="instagram" />
				</a>
			</li>
		</ul>
	</div>
</footer>

<style>
	footer {
		width: 100%;
		max-width: 1000px;
		margin: 0 auto;
		margin-top: 10rem;
		border-top: var(--color-ghost-0) 2px solid;
		font-family: var(--font-mono);
		font-size: 1.2rem;
	}

	.container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 3rem 3rem;
	}

	ul {
		list-style: none;
		display: flex;
		gap: 1.5rem;
	}

	a {
		color: var(--color-black-0);
	}

	a img {
		height: 30px;
		width: auto;
	}

	@media (max-width: 1100px) {
		footer {
			max-width: calc(100% - 6rem);
			font-size: 1.1rem;
		}
		.container {
			padding: 2rem 2rem;
		}
	}

	@media (max-width: 768px) {
		footer {
			max-width: 100%;
			margin-top: 5rem;
			font-size: 1rem;
		}

		a img {
			height: 25px;
			width: auto;
		}
	}

	@media (max-width: 500px) {
		.container {
			flex-direction: column;
			gap: 1rem;
			align-items: start;
		}
	}
</style>
