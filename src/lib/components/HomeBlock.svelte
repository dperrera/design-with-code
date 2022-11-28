<script lang="ts">
	import { onMount } from 'svelte';
	import Key from './Key.svelte';

	export let char: string;
	export let title: string;
	export let subtitle: string;
	export let color = 'blue';

	let cardClasses: string;
	let subtitleClasses: string;
	let keyClasses: string;

	function findCardColor() {
		let colorClass =
			'group bg-white dark:bg-black border-4 aspect-[3/1] flex items-center transition-colors duration-300';
		switch (color) {
			case 'blue':
				return `${colorClass} text-blue-600 border-blue-600 hover:text-white hover:bg-blue-600`;
			case 'teal':
				return `${colorClass} text-teal-500 border-teal-500 hover:text-white hover:bg-teal-500`;
			case 'rose':
				return `${colorClass} text-rose-500 border-rose-500 hover:text-white hover:bg-rose-500`;
		}
		return `${colorClass} text-blue-600 border-blue-600 hover:text-white hover:bg-blue-600`;
	}

	function findSubtitleColor() {
		let colorClass = 'block transition-colors duration-300';
		switch (color) {
			case 'blue':
				return `${colorClass} text-blue-200 dark:text-blue-600/50 group-hover:text-blue-400`;
			case 'teal':
				return `${colorClass} text-teal-200 dark:text-teal-500/40 group-hover:text-teal-300`;
			case 'rose':
				return `${colorClass} text-rose-300 dark:text-rose-500/40 group-hover:text-rose-300`;
		}
		return `${colorClass} text-blue-600 border-blue-600 hover:text-white hover:bg-blue-600`;
	}

	function findKeyColor() {
		let colorClass =
			'group-hover:border-white group-hover:text-white text-[42px] sm:text-7xl font-[300] w-20 h-20 sm:h-40 sm:w-40 duration-300';
		switch (color) {
			case 'blue':
				return `${colorClass} border-blue-600 text-blue-600`;
			case 'teal':
				return `${colorClass} border-teal-500 text-teal-500 `;
			case 'rose':
				return `${colorClass} border-rose-500 text-rose-500 `;
		}
		return `${colorClass} border-blue-600 text-blue-600`;
	}

	onMount(() => {
		cardClasses = findCardColor();
		subtitleClasses = findSubtitleColor();
		keyClasses = findKeyColor();
	});
</script>

<div class={cardClasses}>
	<div class="flex-1 text-2xl sm:text-4xl lg:text-6xl sm:font-light p-4 sm:p-12">
		{title}<span class={subtitleClasses}>{subtitle}</span>
	</div>
	<div class="p-4 sm:p-12">
		<Key {char} class={keyClasses} />
	</div>
</div>
