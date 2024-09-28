<script lang="ts">
	import gradient0 from '$lib/images/gradient-0.webp';
	import gradient0_fallback from '$lib/images/gradient-0.png';

	const questionAnswers = [
		{
			question: 'How do I become a member?',
			answer: 'You can become a member by signing up on our website.'
		},
		{
			question: 'How do I become a member?',
			answer: 'You can become a member by signing up on our website.'
		},
		{
			question: 'How do I become a member?',
			answer: 'You can become a member by signing up on our website.'
		},
		{
			question: 'How do I become a member?',
			answer: 'You can become a member by signing up on our website.'
		}
	];

	const questionCount = questionAnswers.length;
	let showDetails: boolean[] = Array(questionCount).fill(false);

	const toggleDetails = (index: number) => {
		showDetails[index] = !showDetails[index];
	};
</script>

<section>
	<div class="faq-container">
		<picture class="faq-bg">
			<source srcset={gradient0} type="image/webp" />
			<img src={gradient0_fallback} alt="heriozn faq" />
		</picture>

		<h2>Frequently Asked Questions</h2>
	</div>

	<ul>
		{#each questionAnswers as qa, index}
			<li>
				<button class="toggle-wrapper" on:click={() => toggleDetails(index)}>
					<p class="question">{qa.question}</p>
					<span class="toggle-question">{showDetails[index] ? '-' : '+'}</span>
				</button>
				<div class={`answer ${showDetails[index] ? '' : 'hide-answer'}`}>{qa.answer}</div>
			</li>
		{/each}
	</ul>
</section>

<style>
	.faq-container {
		margin: 3rem 0;
		position: relative;
		color: var(--color-white-0);
	}

	.faq-bg {
		width: 100%;
		display: block;
	}

	.faq-bg img {
		width: 100%;
		height: 230px;
		object-fit: cover;
		border-radius: 10px;
	}

	.faq-container h2 {
		position: absolute;
		bottom: 3rem;
		left: 7rem;
		font-size: 2.5rem;
		font-weight: 700;
		filter: drop-shadow(0 1px 4px var(--color-shadow-0));
	}

	ul {
		list-style-type: none;
		font-family: var(--font-mono);
	}

	li {
		border-top: var(--color-ghost-0) 2px solid;
		padding: 1.3rem 4rem;
	}

	.bottom-bar {
		border-bottom: var(--color-ghost-0) 2px solid;
	}

	.toggle-wrapper {
		position: relative;
		padding-right: 3rem;
		display: block;
		width: 100%;
		background: none;
		border: none;
		text-align: start;
		cursor: pointer;
	}

	.question {
		font-size: 1.5rem;
	}

	.toggle-question {
		position: absolute;
		top: -1.3rem;
		right: 0;
		font-size: 3.75rem;
		font-weight: 400;
		font-family: var(--font-mono);
	}

	.answer {
		transition:
			max-height 0.5s,
			opacity 0.2s;
		max-height: 400px;
		overflow: hidden;
		opacity: 1;
	}

	.hide-answer {
		max-height: 0;
		opacity: 0;
	}
</style>
