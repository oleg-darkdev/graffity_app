<script>
  const logos = [
    {
      title: 'montanacolors',
      link: 'https://www.montanacolors.com/en/',
      img: 'https://supernovasmokeshop.com/wp-content/uploads/2016/10/mtn-logo.png'
    },
    {
      title: 'grog inks',
      link: 'https://www.grog.eu/full-metal-paint-line/',
      img: 'https://www.dmentalgraffitishop.com/wp-content/uploads/2017/10/logo-grog.jpg'
    },
    {
      title: '',
      link: '',
      img: ''
    },
    {
      title: '',
      link: '',
      img: ''
    },

  ]
</script>

<div  class="mx-auto  flex flex-row flex-wrap justify-end px-4 py-24">
    {#each logos as logo}
		<a href="{logo.link}" class="bg-primary-light flex items-center justify-center bg-opacity-25 p-6">
			<img src="{logo.img}" alt="{logo.title}" class="block h-20 w-40 object-contain" />
    </a>
    {/each}
</div>
