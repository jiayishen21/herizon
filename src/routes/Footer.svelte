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
				<a href="">
					<img src={linkedin} alt="linkedin" />
				</a>
			</li>
			<li>
				<a href="">
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
	}
</style>
