<script>
	export let style;
</script>

<div class="rounded-lg px-2 py-4" style="background-color: {style.color};">
	<a href={style.link}>
		<img
			src={style.img}
			class="mb-5 h-56 w-full rounded bg-center object-cover"
			alt={style.title}
			loading="lazy"
		/>
	</a>
	<p class="mb-2 text-xs font-semibold uppercase tracking-wider text-neutral-700">{style.title}</p>
	<h2 class="mb-2 text-xl font-bold leading-snug text-neutral-900">
		<a href={style.wikiLink} class="text-neutral-900 hover:text-purple-700">Wikipedia likn &</a>
	</h2>
	{#each style.desc as desc}
		<p class="mb-4 text-sm font-normal text-neutral-900">
			{desc}
		</p>
	{/each}
	<a href={style.link} class="min-w-sm btn-lg btn mt-8">Go to</a>
</div>
