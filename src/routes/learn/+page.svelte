<script lang="ts">
	import HomeBlock from '$lib/components/HomeBlock.svelte';
	import { fade } from 'svelte/transition';
</script>

<div transition:fade={{ delay: 300 }} class="pb-32">
	<div class="max-w-screen-xl mx-auto py-8 px-4 md:px-8">
		<div class="fixed top-8 z-10">
			<a href="/" data-sveltekit-noscroll>
				<h1 class="text-md md:text-xl mb-10 text-blue-600 dark:text-white">Design With Code</h1>
			</a>
		</div>
	</div>

	<div class="max-w-screen-xl mx-auto py-8 px-4 md:px-8">
		<HomeBlock char="✐" title="Get Started" subtitle="Learn the Tools" color="teal" />

		<div class="pt-16">
			<p class="text-2xl md:text-4xl font-light max-w-4xl mb-6 leading-tight">
				Learning to code is all about understanding a few core principles of a language and then
				knowing how to use the internet as a reference to accomplish what you're trying to do.
			</p>

			<div class="prose">
				<p>
					Just like you don't know every word in the dictionary, you won't remember every tag in
					HTML or every property in CSS. Get comfortable searching for what you want to achieve and
					learn as you go.
				</p>

				<p>
					Remember, people made these tools for someone like you to make extraordinary things, and
					you can do it.
				</p>

				<h2>Fundamentals</h2>
				<p>
					The key pieces you'll need to understand are HTML and CSS. MDN's <a
						class="underline hover:line-through"
						href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web"
						target="_blank"
						rel="noreferrer">Getting Started with the web</a
					> is a good, free resource to get you started until DWC's own tutorials are ready.
				</p>
			</div>
		</div>
	</div>
</div>

<style>
	h2 {
		@apply text-2xl md:text-3xl font-light mb-6 mt-10 text-teal-500;
	}
	.prose p {
		@apply max-w-md mb-6;
	}
</style>
