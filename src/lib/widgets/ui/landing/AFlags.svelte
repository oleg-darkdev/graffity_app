<script>
  import { ShowAllDataBtn } from "../../../entities";

	const flags = [
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: [
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
				''
			],
			id: 'lorem',
			img: ''
		}
	];

  let showAll = false;
</script>

<section class="bg-rose-600">
	<div id="world" class="py-12 mx-auto flex max-w-7xl flex-col items-center px-5  sm:px-6 lg:px-8">
		<div class="prose-blue prose mx-auto flex w-full max-w-3xl flex-col text-left">
			<div class="text-white w-full">
				<h2 style="line-height: 0.8em;" class="m-0 text-white font-grafitty text-8xl ">A small headline to switch your visitors into users.</h2>
				<!-- <h3 style="line-height: 0.8em;" class="text-white font-grafitty text-7xl">A small headline to switch your visitors into users.</h3> -->
				<p class="text-white">
					Right. Say that again. No, no, George, look, it's just an act, right? Okay, so 9:00 you're
					strolling through the parking lot, you see us struggling.
				</p>
			</div>
		</div>
		{#each showAll ? flags: flags.slice(0,3) as flag}
			<div
				class="mx-auto my-2 flex max-w-7xl  flex-col items-center border-b border-gray-200 pb-4 sm:flex-row"
			>
				<div
					class="inline-flex h-20 w-20 flex-shrink-0 items-center justify-center rounded-full bg-gray-50 text-neutral-600 sm:mr-10"
				>
					<svg
						fill="none"
						stroke="currentColor"
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="1.5"
						class="h-10 w-10"
						viewBox="0 0 24 24"
					>
						<path stroke="none" d="M0 0h24v24H0z" fill="none" />
						<circle cx="12" cy="12" r="9" />
						<line x1="3.6" y1="15" x2="14.15" y2="15" />
						<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(72 12 12)" />
						<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(144 12 12)" />
						<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(216 12 12)" />
						<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(288 12 12)" />
					</svg>
				</div>

				<div class="prose-md prose mt-6 flex-grow text-center sm:mt-0 sm:text-left">
					<h2 style="line-height: 0.8em;" class="text-white font-grafitty text-7xl m-0">{flag.title}</h2>
					{#each flag.desc as desc}
						<p class="text-white">
							{desc}
						</p>
					{/each}
				</div>
			</div>
		{/each}

      <ShowAllDataBtn link='#world' bind:showAll text='Show all world' />
	</div>
</section>
