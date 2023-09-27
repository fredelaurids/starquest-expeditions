<script>
    
    import Button from './button.svelte';
    
    export let destination = "Edenia Prime";
    export let pricePerPerson = 0;
    export let travelTime = '7 to 10';
    export let image = 'stars.avif';
</script>

<div class="mb-5 overflow-hidden rounded-2xl bg-blue-950 text-blue-100">
	<figure class="no-scrollbar h-[38rem] overflow-y-scroll">
	  <!-- Image -->
	  <img src="{image}" alt="Destination" class="h-2/3 w-full object-cover" />
  
	  <!-- Caption -->
	  <figcaption class="border-t border-blue-800 p-5">
		<!-- Destination Name -->
		<h2 class="mt-1 text-2xl font-bold text-blue-300">{destination}</h2>
  
		<!-- Quick Overview -->
		<div class="my-6 flex flex-row flex-wrap justify-around border-y border-blue-800 px-1 py-3 text-sm text-blue-300 gap-3">
		  <!-- Travel Price -->
		  <div class="flex flex-col items-center basis-1/3 text-center shrink-0 min-w-[110px]">
			<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-6 w-6">
			  <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v12m-3-2.818l.879.659c1.171.879 3.07.879 4.242 0 1.172-.879 1.172-2.303 0-3.182C13.536 12.219 12.768 12 12 12c-.725 0-1.45-.22-2.003-.659-1.106-.879-1.106-2.303 0-3.182s2.9-.879 4.006 0l.415.33M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
			</svg>
			<p>${pricePerPerson} per person</p>
		  </div>
  
		  <!-- Travel Time -->
		  <div class="flex flex-col items-center basis-1/3 text-center shrink-0 min-w-[110px]">
			<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-6 w-6">
			  <path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6h4.5m4.5 0a9 9 0 11-18 0 9 9 0 0118 0z" />
			</svg>
			<p>{travelTime} Earth hours</p>
		  </div>
		</div>
  
		<!-- Description -->
		<div class="flex flex-col gap-2.5">
		  <slot />
		</div>
	  </figcaption>
	</figure>
	<div class="flex flex-row items-center justify-between border-t border-blue-800 p-5 shadow-2xl shadow-black gap-2.5">
	  <Button link="#">Book now</Button>
	  <div class="text-yellow-400 text-right">
		<p class="font-semibold">${pricePerPerson}<span class="text-sm font-normal">/per person</span></p>
	  </div>
	</div>
  </div>