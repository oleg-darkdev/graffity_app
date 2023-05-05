<script>
	import {
		Hero,
		AFlags,
		Header,
		Preview,
		Styles,
		Persons,
		BecomePartner,
		Author
	} from '../lib/widgets';
	import { Logos } from '../lib/entities';
</script>

<Preview />

<section class="flex w-full flex-row flex-wrap">
	<Header />
	<Logos />
</section>
<main class=" content flex-1 overflow-y-scroll">
	<BecomePartner />

	<!-- сюда вставить что-то пустое и занимающее дофига места -->
	<Persons />
	<AFlags />
	<Hero />
	<Styles />
	<Author />
</main>

<style>
</style>
