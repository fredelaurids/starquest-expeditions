<script>
	import Section from '../components/section.svelte';
	import Button from '../components/button.svelte';
	import FlexRow from '../components/flex-row.svelte';
	import FlexRowItem from '../components/flex-row-item.svelte';
</script>

<svelte:head>
    <title>StarQuest Expeditions</title> 
</svelte:head>

<Section bgImage="./stars.avif" fullscreen>
	<h1 class="text-4xl font-bold mb-10">
		Welcome to<br /><span class="text-yellow-400">StarQuest Expeditions</span>
	</h1>
	<h3 class="text-xl font-bold mb-auto">Your portal to the cosmos</h3>

    <FlexRow>
        <FlexRowItem>
            <p>Embark on the journey of a lifetime with the pioneers of intergalactic travel. Discover exotic planets, meet diverse alien civilizations, and forge memories that span the stars.</p>
        </FlexRowItem>
        <FlexRowItem>
            <p>Whether you seek adventure, wonder, or spiritual enlightenment, our state-of-the-art starship, the Stellar Voyager, awaits to carry you into the unknown.</p>
        </FlexRowItem>
        <FlexRowItem>
            <p>Explore the universe.<br>Expand your horizons.<br>Experience the future of travel with <span class="text-yellow-400">StarQuest Expeditions</span>.</p>
        </FlexRowItem>
    </FlexRow>

	<div class="mt-auto">
		<Button link="/destinations">Visit new worlds</Button>
	</div>
</Section>