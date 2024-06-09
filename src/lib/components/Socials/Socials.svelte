<script>
	import ContentLayout from '$lib/utils/ContentLayout.svelte';
</script>

<ContentLayout>
	<div id="socials" class="flex md:flex-row flex-col px-7 gap-10 pt-48">
		<div class="order-2 md:order-1">
			<img class="md:h-[40rem] animate-pulse delay-700" src="/router3.png" alt="router 3" />
		</div>
		<section class="text-right order-1 md:order-2">
			<h3 class="text-3xl sm:text-5xl font-medium mb-7">All you can eat is Treat</h3>
			<p class=" text-xl sm:text-2xl">
				Don't miss out on the joy of owning plenty of $MARTIN tokens {'–'} it's like discovering the
				perfect router treat on Solana.
			</p>

			<p class="text-3xl mt-7">Contract:</p>
			<p class=" text-lg sm:text-2xl">0x000000000000000000000000000000</p>
			<div class="flex gap-3 mt-9 justify-end">
				<img class="w-16 h-16" src="/telegram.svg" alt="telegram icon" />
				<img class="w-16 h-16" src="/twitter.png" alt="twitter icon" />
			</div>
		</section>
	</div>
</ContentLayout>
