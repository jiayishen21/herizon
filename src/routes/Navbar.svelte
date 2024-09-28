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
				<a href="contact">Contact</a>
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
		font-size: 1.2rem;
	}

	.logo {
		width: 45px;
		height: 45px;
	}

	a {
		text-decoration: none;
		color: var(--color-black-0);
	}
</style>
