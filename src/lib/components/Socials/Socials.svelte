<script>
	import ContentLayout from '$lib/utils/ContentLayout.svelte';
</script>

<ContentLayout>
	<div id="socials" class="flex md:flex-row flex-col px-7 gap-10 pt-48">
		<div class="order-2 md:order-1">
			<img class="md:max-h-[40rem] animate-pulse delay-700" src="/router3.png" alt="router 3" />
		</div>
		<section class="text-right order-1 md:order-2">
			<h3 class="text-3xl sm:text-5xl font-medium mb-7">
				Accept dips,but never lose hope in crypto $Router.
			</h3>
			<!-- <p class=" text-xl sm:text-2xl">The blockchain bends toward decentralization</p>-->

			<p class="text-3xl mt-7">Contract:</p>
			<p class=" text-lg sm:text-2xl">0x000000000000000000000000000000</p>
			<div class="flex gap-3 mt-9 justify-end">
				<a href="/"><img class="w-16 h-16" src="/telegram.svg" alt="telegram icon" /></a>
				<a href="/">
					<img class="w-16 h-16" src="/twitter.png" alt="twitter icon" />
				</a>
			</div>
		</section>
	</div>
</ContentLayout>
