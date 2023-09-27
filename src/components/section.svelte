<script>
	export let bgImage = null;
	export let fullscreen = false;
</script>

{#if bgImage != null}
	<section
		class="bg-cover w-full {fullscreen ? 'h-screen' : 'h-auto'}"
		style="background-image: url('{bgImage}')"
	>
		<div class="container py-20 max-w-screen-xl m-auto px-10 2xl:px-0 flex flex-col h-full">
			<slot />
		</div>
	</section>
{:else}
	<section
		class="w-full {fullscreen ? 'h-screen' : 'h-auto'}"
	>
		<div class="container pt-20 max-w-screen-xl m-auto px-10 2xl:px-0 flex flex-col h-full">
			<slot />
		</div>
	</section>
{/if}
