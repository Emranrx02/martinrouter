<script>
	import NavBar from '$lib/components/NavBar/NavBar.svelte';
	import '../app.css';
</script>

<svelte:head>
	<title>Martin Router</title>
	<meta name="Martin Router" content="noindex nofollow" />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Oswald:wght@200..700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>
<section class="font-display">
	<NavBar />
	<slot />
</section>
