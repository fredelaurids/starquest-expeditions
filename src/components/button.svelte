<script>
    export let link;
</script>

<a href="{link}" class="px-4 py-3 bg-teal-400 rounded-md justify-center items-center gap-2.5 inline-flex hover:bg-teal-300 transition-colors duration-300">
	<div class="text-black text-base font-semibold font-['Inter'] leading-snug">
        <span class="whitespace-nowrap">
            <slot />
        </span>
    </div>
</a>
