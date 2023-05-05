<script>
	import '../app.css';
	// import 'aos/dist/aos.css';
	// import AOS from 'aos';
	// import { onMount } from 'svelte';
	// onMount(() => {
	// 	AOS.init();
	// });
</script>

<slot />

<style>
	:global(.font-grafitty) {
		font-family: 'Grafitty';
		line-height: 1.2;
	}

	@font-face {
		font-family: 'Grafitty';
		font-style: normal;
		font-weight: 500;

		src: local(''), /* Super Modern Browsers */ url('/fonts/grafitty-style.woff') format('woff'),
			/* Modern Browsers */ url('/fonts/grafitty-style.ttf') format('truetype'),
			/* Safari, Android, iOS */ url('/fonts/grafitty-style.svg') format('svg'); /* Legacy iOS */
	}
</style>
