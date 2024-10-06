<script>
	import application from '$lib/images/timeline/application.webp';
	import application_fallback from '$lib/images/timeline/application.png';
	import email from '$lib/images/timeline/email.webp';
	import email_fallback from '$lib/images/timeline/email.png';
	import meeting from '$lib/images/timeline/meeting.webp';
	import meeting_fallback from '$lib/images/timeline/meeting.png';
	import resource from '$lib/images/timeline/resource.webp';
	import resource_fallback from '$lib/images/timeline/resource.png';
	import consulting from '$lib/images/timeline/consulting.webp';
	import consulting_fallback from '$lib/images/timeline/consulting.png';
</script>

<section>
	<h2>Onboarding is easy.</h2>
	<p class="subtitle">Hover on each step to see details</p>

	<div class="timeline">
		<div></div>
		<div class="timeline-middle">
			<div class="timeline-point"></div>
		</div>
		<div class="timeline-component">
			<h4>Step 1: Application</h4>
			<div class="image-container">
				<picture>
					<source srcset={application} type="image/webp" />
					<img src={application_fallback} alt="sign up on our form" />
				</picture>
				<div class="image-desc">
					<p>
						Fill out our <a href="https://tgopp36ovob.typeform.com/to/SlUd9Xpv" target="_blank">
							member application
						</a>
						(3 minutes ETA).
					</p>
				</div>
			</div>
		</div>

		<div class="timeline-component">
			<h4>Step 2: Email Introduction</h4>
			<div class="image-container">
				<picture>
					<source srcset={email} type="image/webp" />
					<img src={email_fallback} alt="sign up on our form" />
				</picture>
				<div class="image-desc">
					<p>We'll send an email with details about the membership process and our resources.</p>
				</div>
			</div>
		</div>
		<div class="timeline-middle">
			<div class="timeline-point"></div>
		</div>
		<div></div>

		<div></div>
		<div class="timeline-middle">
			<div class="timeline-point"></div>
		</div>
		<div class="timeline-component">
			<h4>Step 3: “Get-to-know you” meeting</h4>
			<div class="image-container">
				<picture>
					<source srcset={meeting} type="image/webp" />
					<img src={meeting_fallback} alt="sign up on our form" />
				</picture>
				<div class="image-desc">
					<p>Tell us about your business progress, plans, and needs in an initial meeting.</p>
				</div>
			</div>
		</div>

		<div class="timeline-component">
			<h4>Step 4: Resource matching</h4>
			<div class="image-container">
				<picture>
					<source srcset={resource} type="image/webp" />
					<img src={resource_fallback} alt="sign up on our form" />
				</picture>
				<div class="image-desc">
					<p>
						We'll match you with resources and opportunities that align with your business goals.
					</p>
				</div>
			</div>
		</div>
		<div class="timeline-middle">
			<div class="timeline-point"></div>
		</div>
		<div class="timeline-component"></div>

		<div class="timeline-component"></div>
		<div class="timeline-middle">
			<div class="timeline-point"></div>
			<div class="timeline-point timeline-point-bottom"></div>
		</div>
		<div class="timeline-component">
			<h4>Step 5: Consultation & advising</h4>
			<div class="image-container">
				<picture>
					<source srcset={consulting} type="image/webp" />
					<img src={consulting_fallback} alt="sign up on our form" />
				</picture>
				<div class="image-desc">
					<p>
						Connect with industry experts and get personalized advice on your business strategy,
						marketing, and more.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	section {
		margin-top: 2.5rem;
	}

	h2 {
		font-size: 3rem;
		font-weight: 700;
		text-align: center;
	}

	.subtitle {
		font-family: var(--font-mono);
		color: var(--color-ghost-1);
		text-align: center;
		font-size: 1.2rem;
		font-weight: 400;
		margin-top: 1rem;
	}

	.timeline {
		max-width: 900px;
		margin: 4rem auto;
		display: grid;
		grid-template-columns: 1fr 3px 1fr;
	}

	.timeline-component {
		margin: 0 20px 20px 20px;
	}

	h4 {
		font-size: 1.5rem;
		font-weight: 400;
		font-family: var(--font-mono);
	}

	.timeline-middle {
		position: relative;
		background: var(--color-black-0);
	}

	.timeline-point {
		position: absolute;
		top: 0;
		left: 50%;
		transform: translateX(-50%);
		width: 15px;
		height: 15px;
		background: var(--color-black-0);
		border-radius: 50%;
	}

	.timeline-point-bottom {
		top: initial;
		bottom: 0;
	}

	.image-container {
		margin-top: 0.5rem;
		height: 180px;
		position: relative;
	}
	.image-container img {
		width: 100%;
		height: 180px;
		object-fit: cover;
		border-radius: 10px;
	}

	.image-desc {
		position: absolute;
		top: 0;
		left: 0;
		height: 100%;
		background: var(--color-shadow-0);
		backdrop-filter: blur(10px);
		color: var(--color-white-0);
		font-size: 1.2rem;
		z-index: 1;
		padding: 2rem;
		border-radius: 10px;

		opacity: 0;
		transition: opacity 0.3s ease-out;
	}

	.image-desc a {
		color: var(--color-link-0);
	}

	.image-container:hover .image-desc {
		opacity: 1;
	}

	@media (max-width: 1300px) {
		h2 {
			font-size: 2.5rem;
		}

		.subtitle {
			font-size: 1.1rem;
		}

		h4 {
			font-size: 1.4rem;
		}
	}

	@media (max-width: 950px) {
		h2 {
			font-size: 2rem;
		}

		.subtitle {
			font-size: 1rem;
		}

		h4 {
			font-size: 1.3rem;
		}

		.image-container .image-desc {
			font-size: 1.1rem;
			padding: 1rem;
		}
	}

	@media (max-width: 768px) {
		h2 {
			font-size: 1.75rem;
		}

		h4 {
			font-size: 1.1rem;
		}

		.subtitle {
			display: none;
		}

		.image-container img {
			display: none;
		}

		.image-container {
			height: fit-content;
		}

		.image-container .image-desc {
			position: relative;
			background: none;
			margin-top: 1rem;
			font-size: 1rem;
			opacity: 1;
			padding: 0;
			color: var(--color-black-0);
		}

		.timeline {
			margin: 2rem auto;
		}
	}
</style>
