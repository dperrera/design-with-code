<script lang="ts">
	let clazz: string;
	export { clazz as class };
	export let char: string;
</script>

<div
	class={`text-blue-600 border-blue-600 hover:text-blue-300 hover:border-blue-300 dark:hover:text-white dark:hover:border-white transition-colors duration-700 flex items-center justify-center border-4 rounded-lg ${clazz}`}
>
	{char}
</div>
