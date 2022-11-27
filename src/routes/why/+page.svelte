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
		<HomeBlock char="‽" title="Why Code?" subtitle="The Manifesto" color="blue" />

		<div class="pt-16">
			<p class="text-2xl md:text-4xl font-light max-w-4xl mb-6 leading-tight">
				When designing software, a website, or anything else that exists on a screen – code is the
				best design tool for the job.
			</p>

			<p class="text-2xl md:text-4xl font-light max-w-4xl mb-6 leading-tight">
				Nothing else lets you experience your work as you make it.
			</p>

			<div class="prose">
				<p>
					The benefits of adding code to your design toolbox are vast, but if you're still on the
					fence, here's what you can expect when incorporating code into your design process:
				</p>

				<h2>Better decisions, faster.</h2>

				<p>
					The "X" in "UX" stands for "experience." If you're making static comps and stitching them
					together, are you experiencing anything?
				</p>

				<p>
					Imagine instead a world where you can shorten your feedback loop. You can iterate over
					interactions before anyone else sees them.
				</p>

				<h2>Higher quality feedback.</h2>

				<p>
					Since your design is in code, you can do amazing things with it. You can throw it on the
					internet, show it around, and get high-quality feedback from your customers and prospects.
				</p>

				<p>
					So, now not only will you be able to express your vision where people will experience it,
					but you'll take a considerable amount of risk off the table when you introduce rapid
					prototyping and user testing into your process.
				</p>

				<h2>The best learning investment.</h2>

				<p>
					"Code" has been the domain of developers and engineers, but it's not magic. It's simply a
					way that we humans can tell computers what to do. We can go quite a long way with just
					HTML and CSS. When you're ready, JavaScript will give you interaction superpowers.
				</p>

				<p>
					The critical thing to remember is that everything you learn in this domain builds on each
					other. You don't need to worry about code getting acquired or going out of business. These
					tools have been around and steadily improving for decades, and they're at the foundation
					of the internet – meaning they'll likely be here after we're all gone.
				</p>

				<h2>Why now?</h2>

				<p>
					Over the last ten years, "design tools" have become far more complex, while "developer
					tools" have become far more approachable and are infinitely more powerful. You could even
					argue that they have a better user interface.
				</p>

				<p>
					Designers, it's time to get some better tools. If we have to steal them from our developer
					friends, so be it; everything we'll talk about here is free or open source anyway– they
					won't mind.
				</p>

				<p>
					Ready to get started? Head over to the <a href="/guides">Field Guide</a>
					to get started.
				</p>
			</div>
		</div>
	</div>
</div>

<style>
	h2 {
		@apply text-2xl md:text-3xl font-light mb-6 mt-10 text-blue-600;
	}
	.prose p {
		@apply max-w-md mb-6;
	}
</style>
