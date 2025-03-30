<script>
	import DonateIcon from '$lib/icons/socials/donate.svelte';
	import GitHubIcon from '$lib/icons/socials/github.svelte';
	import LinkedInIcon from '$lib/icons/socials/linkedin.svelte';
	import MusicIcon from '$lib/icons/socials/soundcloud.svelte';
	import MastodonIcon from '$lib/icons/socials/mastodon.svelte';
</script>

<div class="socials">
	<a
		href="https://www.linkedin.com/in/lily-o"
		target="_blank"
		rel="noopener noreferrer"
		title="Connect with me on LinkedIn"
	>
		<LinkedInIcon />
	</a>
	<a
		href="https://ko-fi.com/lily_neinhorn"
		target="_blank"
		rel="noopener noreferrer"
		title="Support me on Ko-fi"
	>
		<DonateIcon />
	</a>
	<a
		href="https://github.com/lily-gh"
		target="_blank"
		rel="noopener noreferrer"
		title="See my GitHub profile"
	>
		<GitHubIcon />
	</a>
	<a
		href="https://soundcloud.com/lily_neinhorn"
		target="_blank"
		rel="noopener noreferrer"
		title="Listen to my crazy music ideas"
	>
		<MusicIcon />
	</a>
</div>

<style lang="scss">
	@import '../../scss/breakpoints.scss';
	.socials {
		display: flex;
		align-items: center;
		gap: 20px;

		a {
			transition: all 0.2s ease-in-out;
			width: 24px;
			color: var(--color--text);
			fill: var(--color--text);

			&:hover {
				color: var(--color--primary);
				fill: var(--color--primary);
				filter: drop-shadow(0px 0px 3px var(--color--primary));
			}
		}
	}
</style>
