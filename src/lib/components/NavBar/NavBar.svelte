<script lang="ts">
	import ContentLayout from '$lib/utils/ContentLayout.svelte';
	import classNames from 'classnames';
	import { onMount } from 'svelte';
	import { Hamburger } from 'svelte-hamburgers';

	const navItem = [
		{ name: 'home', slug: 'dex-tools' },
		{ name: 'Socials', slug: 'dex-tools' },
		{ name: 'Dream?', slug: 'dex-tools' },
		{ name: 'Tokenomics', slug: 'dex-tools' }
	];

	let open = false;
	let body: HTMLBodyElement | undefined;

	onMount(() => {
		//@ts-ignore
		body = document.getElementsByTagName('BODY')[0];
	});

	$: {
		if (body && open) {
			//@ts-ignore
			body.style = 'overflow: hidden';
		} else if (body)
			//@ts-ignore
			body.style = 'overflow-y: auto';
	}
</script>

<section class="bg-[#FEE0C9]">
	<ContentLayout>
		<section class="flex py-5 sm:py-11 sm:px-16 items-center">
			<img src="/router.png" alt="marting router logo" class=" w-28 lg:w-40 mr-2 mb-11" />
			<p class=" uppercase text-xl sm:text-3xl lg:text-5xl font-bold">Marting Router</p>

			<ul class=" md:flex hidden font-medium gap-5 ml-auto text-base lg:text-xl">
				{#each navItem as item}
					<li class="uppercase cursor-pointer">{item.name}</li>
				{/each}
			</ul>

			<div class="md:hidden ml-auto block">
				<Hamburger bind:open --color="black" />
			</div>

			<div
				role="button"
				tabindex="0"
				on:keydown
				on:click={() => {
					open = false;
				}}
				class={classNames(
					'fixed overflow-hidden transition-transform top-0 left-0 w-full h-[100vh] backdrop-blur-sm',
					open ? 'translate-x-0' : 'translate-x-[100%]'
				)}
			>
				<ul
					class={classNames(
						'flex  bg-gray-600 transition-transform  delay-300 ease-in-out px-10 py-20 h-full text-white top-0 right-0 absolute flex-col font-medium gap-5  text-base lg:text-xl',
						open ? 'translate-x-0' : 'translate-x-[100%]'
					)}
				>
					{#each navItem as item}
						<li class="uppercase cursor-pointer">{item.name}</li>
					{/each}
				</ul>
			</div>
		</section>
	</ContentLayout>
</section>
