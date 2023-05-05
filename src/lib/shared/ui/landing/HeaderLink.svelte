<script>
  export let link;
</script>

<li class="h-16">
	<a
		href="{link.link}"
		class="border-b-2 border-transparent px-2 py-1 text-6xl font-grafitty  text-neutral-900 hover:border-neutral-900 hover:text-neutral-900 md:px-3 lg:px-6"
	>
		<span class="hidden lg:inline">{link.title} </span>
	</a>
</li>
