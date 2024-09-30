<script>
	import logo from '$lib/images/herizon-logo.png';
</script>

<nav>
	<div class="container">
		<a href="/">
			<img src={logo} alt="Herizon" class="logo" />
		</a>

		<ul>
			<li>
				<a href="mailto:herizon@gmail.com" target="_blank">Contact</a>
			</li>
			<li>
				<a href="join">Join us</a>
			</li>
		</ul>
	</div>
</nav>

<style>
	nav {
		width: 100%;
		max-width: 1000px;
		margin: 0 auto;
		border-bottom: var(--color-ghost-0) 2px solid;
		font-size: 1.2rem;
	}

	.container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0.5rem 6rem;
	}

	ul {
		list-style: none;
		font-family: var(--font-mono);
		display: flex;
		gap: 3rem;
	}

	.logo {
		width: 45px;
		height: 45px;
	}

	a {
		text-decoration: none;
		color: var(--color-black-0);
	}

	@media (max-width: 1100px) {
		nav {
			max-width: calc(100% - 6rem);
			font-size: 1.1rem;
		}

		.container {
			padding: 0.5rem 3rem;
		}
	}

	@media (max-width: 768px) {
		nav {
			max-width: 100%;
			font-size: 1rem;
		}

		.logo {
			width: 40px;
			height: 40px;
		}
	}

	@media (max-width: 500px) {
		.container {
			padding: 0.5rem 2rem;
		}

		ul {
			gap: 1.5rem;
		}
	}
</style>
