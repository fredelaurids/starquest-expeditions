<script>
	import Section from '../components/section.svelte';
	import Button from '../components/button.svelte';
</script>

<Section bgImage="./stars.avif" fullscreen>
	<h1 class="text-4xl font-bold mb-10">
		404<br /><span class="text-yellow-400">File not found</span>
	</h1>
	<h3 class="text-xl font-bold">Whatever you were looking for may be lost in space</h3>

	<div class="mt-10">
		<Button link="/">Go to homepage</Button>
	</div>
</Section>