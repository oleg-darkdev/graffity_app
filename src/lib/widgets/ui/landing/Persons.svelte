<script>
	import { PersonCard } from '../../../entities';


	const persons = [
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			link: 'Lorem-ipsum ',
			img: 'https://thumbs.dreamstime.com/b/graffiti-vandal-8900799.jpg',
      bg: '#b91c1c'
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			link: 'Lorem-ipsum ',
			img: 'https://thumbs.dreamstime.com/b/graffiti-vandal-8900799.jpg',
      bg: '#16a34a'
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			link: 'Lorem-ipsum ',
			img: 'https://thumbs.dreamstime.com/b/graffiti-vandal-8900799.jpg',
      bg: '#be123c'
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			link: 'Lorem-ipsum ',
			img: 'https://thumbs.dreamstime.com/b/graffiti-vandal-8900799.jpg',
      bg: '#c026d3'
		}
	];
</script>

<section id='heroes' class="mx-auto flex w-full flex-col items-end px-4 my-12 ">
	<div
		class="grid max-w-5xl grid-cols-1 gap-10 rounded-lg bg-yellow-500 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-3"
	>
		<div class="col-span-1 md:col-span-2 lg:col-span-2 xl:col-span-3">
			<a href="#">
				<img
					src="/images/graffity_bg.png"
					class="mb-5 h-64 w-full rounded bg-center object-cover"
					alt="Kutty"
					loading="lazy"
				/>
			</a>
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

		<div class="mx-auto flex flex-wrap  md:flex-nowrap">
			{#each persons as person}
				<PersonCard {person} />
			{/each}
		</div>
	</div>

</section>
