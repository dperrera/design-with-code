<script lang="ts">
	import '../app.css';
</script>

<svelte:head>
	<title>Design With Code</title>
	<link rel="stylesheet" href="https://rsms.me/inter/inter.css" />

	<meta name="title" content="Design With Code" />
	<meta
		name="description"
		content="A space for designers that use code to bring their ideas to life."
	/>

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://www.designwithcode.org/" />
	<meta property="og:title" content="Design With Code" />
	<meta
		property="og:description"
		content="A space for designers that use code to bring their ideas to life."
	/>
	<meta property="og:image" content="https://www.designwithcode.org/social.png" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://www.designwithcode.org/" />
	<meta property="twitter:title" content="Design With Code" />
	<meta
		property="twitter:description"
		content="A space for designers that use code to bring their ideas to life."
	/>
	<meta property="twitter:image" content="https://www.designwithcode.org/social.png" />
</svelte:head>

<div>
	<slot />
</div>
