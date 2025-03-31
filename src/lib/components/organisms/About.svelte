<script>
	import SparklingHighlight from '$lib/components/molecules/SparklingHighlight.svelte';
	import Socials from '$lib/components/molecules/Socials.svelte';
	import Image from '../atoms/Image.svelte';
</script>

<section id="about">
	<div class="info">
		<h2>
			Where curiosity and creativity meet engineering
			<SparklingHighlight color="secondary">excellence</SparklingHighlight>.
		</h2>
		<p>
			With a decade of experience in software engineering, my goal is to create intuitive,
			high-performing applications while staying creative. <SparklingHighlight color="secondary"
				>#TODO: change</SparklingHighlight
			>.
			<br />
			<br />
			On my free time, I enjoy coding fun projects and bringing quirky ideas to life.
		</p>
		<div class="socials">
			<span>Socials:</span>
			<Socials />
		</div>
	</div>
	<div class="image">
		<Image src="/images/sample-image.png" alt="Sample for the static template" />
	</div>
</section>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#about {
		position: relative;
		display: grid;
		grid-template-columns: 500px 250px;
		align-items: center;
		justify-content: space-between;
		padding-bottom: 50px;

		@include for-phone-only {
			grid-template-columns: 1fr;
			justify-items: center;
			gap: 20px;
		}

		.info {
			display: flex;
			flex-direction: column;
			gap: 10px;
			h2 {
				@include for-phone-only {
					text-align: center;
				}
			}

			p {
				@include for-phone-only {
					text-align: justify;
				}
			}

			@include for-phone-only {
				gap: 20px;
			}
		}

		.socials {
			display: flex;
			align-items: center;
			gap: 15px;

			@include for-phone-only {
				justify-content: center;
				margin-bottom: 10px;
				span {
					display: none;
				}
			}
		}

		.image {
			width: 220px;
			height: 220px;
		}
	}
</style>
