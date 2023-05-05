<script>
	import { onMount } from 'svelte';
	import { HeaderLink } from '../../../shared';

	onMount(async () => {
		const сollaborationElement = document.getElementById('сollaboration'),
			heroesElement = document.getElementById('heroes'),
			stylesElement = document.getElementById('styles'),
			previewElement = document.getElementById('preview'),
			headerElement = document.getElementById('myHeader');

		window.addEventListener('scroll', function () {
			const targetPositionCollaboration = сollaborationElement.getBoundingClientRect().top,
				targetPositionHeroes = heroesElement.getBoundingClientRect().top,
				targetPositionPreview = previewElement.getBoundingClientRect().top,
				targetPositionStyles = stylesElement.getBoundingClientRect().top;

			const windowPosition = window.pageYOffset;

			const distanceCollaboration = targetPositionCollaboration - windowPosition,
				distanceHeroes = targetPositionHeroes - windowPosition,
				distancePreview = targetPositionPreview - windowPosition,
				distanceStyles = targetPositionStyles - windowPosition;

			if (distancePreview <= 0) {
				headerElement.classList.remove(
					'bg-fuchsia-500',
					'border-fuchsia-500',
					'shadow-fuchsia-600',
					'bg-rose-500',
					'border-rose-500',
					'shadow-rose-600',
					'bg-amber-500',
					'border-amber-500',
					'shadow-amber-600'
				);
				headerElement.classList.add('bg-lime-500', 'border-lime-500', 'shadow-lime-600');
			}

			if (distanceCollaboration <= 0) {
				headerElement.classList.remove(
					'bg-amber-500',
					'border-amber-500',
					'shadow-amber-600',
					'bg-lime-500',
					'border-lime-500',
					'shadow-lime-600',
					'bg-fuchsia-500',
					'border-fuchsia-500',
					'shadow-fuchsia-600'
				);
				headerElement.classList.add('bg-rose-500', 'border-rose-500', 'shadow-rose-600');
			}

			if (distanceHeroes <= 0) {
				headerElement.classList.remove(
					'bg-lime-500',
					'border-lime-500',
					'shadow-lime-600',
					'bg-rose-500',
					'border-rose-500',
					'shadow-rose-600',
					'bg-fuchsia-500',
					'border-fuchsia-500',
					'shadow-fuchsia-600'
				);
				headerElement.classList.add('bg-amber-500', 'border-amber-500', 'shadow-amber-600');
			}

			if (distanceStyles <= 0) {
				headerElement.classList.remove(
					'bg-lime-500',
					'border-lime-500',
					'shadow-lime-600',
					'bg-rose-500',
					'border-rose-500',
					'shadow-rose-600',
					'bg-amber-500',
					'border-amber-500',
					'shadow-amber-600'
				);
				headerElement.classList.add('bg-fuchsia-500', 'border-fuchsia-500', 'shadow-fuchsia-600');
			}
		});
	});

	const links = [
		{
			title: 'Web app',
			link: '#'
		},
		{
			title: 'Persons',
			link: '#heroes'
		},
		{
			title: 'Graffity styles',
			link: '#styles'
		},
		{
			title: 'Street-art world',
			link: '#world'
		},
		{
			title: 'Collaboration',
			link: '#сollaboration'
		}
	];

	let open = false;
</script>

<header
	id="myHeader"
	class="header sticky mt-40 h-auto w-3/12 rounded-br-lg rounded-tr-lg border-2 border-lime-500  bg-lime-500 shadow-md shadow-lime-600"
>
	<div
		x-data={open}
		class="mx-auto flex max-w-screen-xl flex-col p-5 md:items-center md:justify-between md:px-6 lg:px-8"
	>
		<div class=" mb-8 flex flex-row items-center justify-between lg:justify-start">
			<a
				href="/"
				class="tracking-relaxed transform text-lg font-bold tracking-tighter transition duration-500 ease-in-out lg:pr-8"
			>
				<img src="/images/logo.png" class="h-34 rounded-lg" alt="Logo" />
			</a>
			<!-- <button
				class="focus:shadow-outline rounded-lg focus:outline-none md:hidden"
				on:click={() => (open = !open)}
			>
				<svg fill="currentColor" viewBox="0 0 20 20" class="h-8 w-8">
					<path
						x-show="!open"
						fill-rule="evenodd"
						d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
						clip-rule="evenodd"
					/>
					<path
						x-show="open"
						fill-rule="evenodd"
						d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
						clip-rule="evenodd"
						style="display: none"
					/>
				</svg>
			</button> -->
		</div>
		<!-- 	-->
		<nav
			class="{open
				? 'flex'
				: 'hidden'} flex flex-grow flex-col md:flex md:flex-row md:justify-start"
		>
			<!-- {#each links as link}
				<a href={link.link}>
					<img src="" class="my-1 h-20 w-40" alt={link.title} />
				</a>
			{/each} -->
			<ul class="flex list-none flex-col space-y-2 lg:inline-flex lg:items-center lg:space-y-0">
				{#each links as link}
					<HeaderLink {link} />
				{/each}
			</ul>
		</nav>
	</div>
</header>

<style>
	.sticky {
		position: fixed;
		top: 0;
	}
</style>
