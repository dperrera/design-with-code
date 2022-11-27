<script>
	import Key from '$lib/components/Key.svelte';
	import HomeBlock from '$lib/components/HomeBlock.svelte';
	import { fade } from 'svelte/transition';
</script>

<div transition:fade>
	<div class="max-w-screen-xl mx-auto py-8 px-4 md:px-8">
		<div class="fixed top-8 z-10">
			<a href="/">
				<h1 class="text-md md:text-xl mb-10 text-blue-700">Design With Code</h1>
			</a>
		</div>
	</div>

	<div class="sticky max-w-screen-xl mx-auto top-24 mb-20  px-4 md:px-8">
		<div class="md:aspect-[3/1] flex items-center p-4 sm:p-12">
			<p
				class="text-2xl sm:text-4xl md:text-5xl lg:text-6xl sm:font-light max-w-sm sm:max-w-xl md:max-w-xl lg:max-w-2xl"
			>
				A space for designers that use code to bring their ideas to life.
			</p>
		</div>
	</div>

	<a class="block max-w-screen-xl mx-auto sticky top-24 mb-8 sm:mb-20 px-4 md:px-8" href="/why">
		<HomeBlock char="‽" title="Why Code?" subtitle="The Manifesto" color="blue" />
	</a>

	<a class="block max-w-screen-xl mx-auto sticky top-28 mb-8 sm:mb-20  px-4 md:px-8" href="/learn">
		<HomeBlock char="✐" title="Get Started" subtitle="Learn the Tools" color="teal" />
	</a>

	<a
		class="block max-w-screen-xl mx-auto sticky top-32 mb-8 sm:mb-20 px-4 md:px-8"
		href="https://designwithcode.substack.com/"
		target="_blank"
		rel="noreferrer"
	>
		<HomeBlock char="☞" title="Subscribe" subtitle="Newsletter" color="rose" />
	</a>

	<div class="sticky top-24 bg-amber-100 dark:bg-neutral-900 py-10 md:py-20">
		<div class="max-w-screen-xl mx-auto px-4 md:px-8">
			<h2
				class="text-2xl sm:text-4xl md:text-5xl lg:text-6xl md:font-light mb-8 text-blue-600 px-4 sm:px-12"
			>
				By Designers. <span class="block opacity-70">For Designers.</span>
			</h2>
			<p class="max-w-prose px-4 sm:px-12">
				Design With Code is made by me, <a
					class="underline hover:line-through"
					href="https://perrera.com">Dan Perrera</a
				>, a design leader, and former teacher, who believes that our industry would be better if
				more designers knew how to code. So here I am – building a space where designers can pick up
				new tools and techniques to empower us to reach new heights in our craft.
			</p>

			<div class="flex flex-col items-center justify-center">
				<div class="aspect-[4/1] flex-none self-stretch " />
				<div class="grid grid-cols-6 gap-4 w-fit mx-auto cursor-default scale-75 sm:scale-50">
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="<" />
					<div class="col-span-5" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="D" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="E" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="S" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="I" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="G" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="N" />
					<div class="col-span-2" />

					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="W" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="I" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="T" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="H" />
					<div class="col-span-1" />

					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="C" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="O" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="D" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="E" />
					<div class="col-span-2" />
					<div class="col-span-2" />

					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char="/" />
					<Key class="h-10 w-10 sm:h-16 sm:w-16 sm:text-2xl font-bold" char=">" />
				</div>
			</div>
		</div>
	</div>
</div>
