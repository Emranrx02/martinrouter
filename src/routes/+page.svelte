<script>
	import Dream from '$lib/components/Dream/Dream.svelte';
	import Header from '$lib/components/Header/Header.svelte';
	import NavBar from '$lib/components/NavBar/NavBar.svelte';
	import Socials from '$lib/components/Socials/Socials.svelte';
	import Tokenomics from '$lib/components/Tokenomics/Tokenomics.svelte';
</script>

<section>
	<section class="bg-[url('/martin.jpeg')]   h-full bg-no-repeat bg-cover bg-center">
	<section class="backdrop-brightness-[.3]">
	<NavBar />
	<Header />
	</section>
	</section>
	<Dream />
	<Tokenomics />
	<Socials/>
</section>
