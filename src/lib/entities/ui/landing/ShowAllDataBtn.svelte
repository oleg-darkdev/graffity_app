<script>
	export let link, showAll, text;
</script>

<button
	on:click={() => {
		showAll = !showAll;
		location.href = { link };
	}}
	class="min-w-sm btn-lg btn mt-8">Show all {text}</button
>
