<script>
	import { ShowAllDataBtn } from '../../../entities';

	const styles = [
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#ea580c',
			reverse: false
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#84cc16',
			reverse: true
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#34d399',
			reverse: false
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#c026d3',
			reverse: true
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#be123c',
			reverse: false
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],
			wikiLink: '',
			color: '#16a34a',
			reverse: true
		},
		{
			link: 'lorem',
			img: 'https://3.bp.blogspot.com/-lbmKq9_C9YI/TwT-a3kxfUI/AAAAAAAAAdo/Y-R0Cesjk_M/s1600/Graffiti-art-font.jpg',
			title: 'Lorem ipsum is placeholder',
			shortDesc:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups. Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			fullDesc: ['', '', ''],

			wikiLink: '',
			color: '#b91c1c',
			reverse: false
		}
	];

	let showAll = false;
</script>

<!--
<section class="mx-auto flex w-full flex-col items-end px-4  ">
	<div class="flex max-w-5xl flex-col rounded-lg bg-yellow-500 px-2 py-6">
		<div class="col-span-1 md:col-span-2 lg:col-span-2 xl:col-span-3">
			<h2 class="mx-4 mb-2 text-end text-3xl font-bold leading-snug ">
				<a href="#" class="text-neutral-900 hover:text-purple-700"
					>Wybierz bohatera, który pasuje do Twojego stylu rysowania</a
				>
			</h2>
			<p class="mx-4 text-end text-sm font-normal text-neutral-900">
				Earlier RPA bots used to have some limitations like it would take structured data for
				processing from excel, database, on these data. But with advancements in technology like OCR
				(Optical Character Recognition) and Machine Learning, RPA bots are capable of extracting
				these data …
			</p>
		</div>
		<div
			id="styles"
			class="my-4 grid grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-3 "
		>
			{#each showAll ? styles : styles.slice(0, 3) as style}
				<StyleCard {style} />
			{/each}
		</div>
		<div class="flex w-full justify-center">
			<ShowAllDataBtn link="#styles" bind:showAll text="Show all styles" />
		</div>
	</div>
</section> -->

<section id="styles" class="relative w-full bg-fuchsia-500 px-4 py-24 ">
	{#each showAll ? styles : styles.slice(0, 3) as style}
		<div
			class="grid grid-cols-1 items-center gap-y-10 gap-x-10 md:grid-cols-2 md:gap-y-32 md:gap-x-24"
		>
			<div class={style.reverse ? 'order-none md:order-2' : ''}>
				<h2
					style="line-height: 0.8em;"
					class="font-grafitty mb-4 text-center text-8xl  tracking-tight text-neutral-900  sm:text-left  md:leading-tight"
				>
					{style.title}
				</h2>
				<p class="mb-5 text-center text-base text-gray-600 sm:text-left md:text-lg">
					{style.shortDesc}
				</p>
				<a href="#" class="btn-dark btn-md btn w-full max-w-md">Learn More</a>
			</div>
			<div class="h-full  w-full rounded-lg bg-gray-200 py-48" />
		</div>
	{/each}

	<div class="flex w-full justify-center">
		<ShowAllDataBtn link="#styles" bind:showAll text="Show all styles" />
	</div>
</section>
