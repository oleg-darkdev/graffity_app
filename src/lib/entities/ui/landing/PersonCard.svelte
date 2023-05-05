<script>
  export let person;
</script>

<a href="{person.link}">
	<div class="flex w-full" >
		<div style='background-color: {person.bg};'
			class="relative m-1 flex transform flex-col items-start rounded-xl bg-white shadow-2xl transition delay-150 duration-300 ease-in-out md:-ml-16 md:w-80 md:hover:-translate-x-16 md:hover:-translate-y-8"
		>
			<img
				class="w-full rounded-t-xl object-cover object-center md:h-36 lg:h-48"
				src="{person.img}"
				alt="{person.title}"
			/>
			<div class="px-6 py-4">
				<h4 class=" text-2xl font-semibold text-neutral-900">
					<span class="">Entry</span>
				</h4>
				<p class="leading-relax mt-4 text-base font-normal text-gray-800">
					{person.desc}
				</p>
			</div>
		</div>
	</div>
</a>
