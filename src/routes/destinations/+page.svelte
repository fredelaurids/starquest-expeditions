<script>
	import Section from '../../components/section.svelte';
	import FlexRow from '../../components/flex-row.svelte';
	import FlexRowItem from '../../components/flex-row-item.svelte';
	import DestinationCard from '../../components/destination-card.svelte';
</script>

<svelte:head>
    <title>StarQuest Expeditions | Destinations</title> 
</svelte:head>


<Section bgImage="./stars.avif">
	<h1 class="text-4xl font-bold mb-10">
		Our <span class="text-yellow-400">destinations</span>
	</h1>

	<FlexRow>
        <FlexRowItem>
            <p>Please keep in mind that these are ballpark figures and that <span class="text-yellow-400">StarQuest Expeditions</span> offers a range of customization options, including different cabin types, extended stays, and exclusive add-ons, which can affect the final cost.</p>
        </FlexRowItem>
        <FlexRowItem>
            <p>Additionally, discounts may be available for group bookings or repeat travelers. Travelers can contact <span class="text-yellow-400">StarQuest Expeditions</span> directly for personalized quotes and to discuss specific preferences for their vacation.</p>
        </FlexRowItem>
    </FlexRow>
</Section>

<Section>
    <div class="grid gap-10 grid-cols-1 sm:grid-cols-2 lg:grid-cols-3">
        <DestinationCard pricePerPerson="10000" travelTime="7 to 10" destination="Edenia Prime">
            <p>
                Edenia Prime is relatively close to the central hub, making it a convenient choice for
                travelers seeking a short interstellar getaway.
            </p>
            <p>
                A lush, biodiverse planet where travelers can explore exotic flora and fauna.
            </p>
            <p>
                Includes guided tours of the biodiverse landscapes, wildlife encounters, and accommodations
                on Edenia Prime.
            </p>
        </DestinationCard>
        <DestinationCard pricePerPerson="12500" travelTime="15 to 20" destination="Nebula Sky Gardens">
            <p>
                The Nebula Sky Gardens are located within a nearby nebula, requiring a slightly longer journey through warp corridors.
            </p>
            <p>
                A space station within a vibrant nebula, offering stunning celestial views.
            </p>
            <p>
                Includes a stay at the Nebula Sky Gardens space station, access to observation decks, and celestial events.
            </p>
        </DestinationCard>
        <DestinationCard pricePerPerson="9500" travelTime="20 to 25" destination="Zephyrion Sands">
            <p>
                Zephyrion Sands is situated on a desert world within a neighboring star system, making it a moderate-distance trip.
            </p>
            <p>
                A desert world with floating sand dunes and ancient alien ruins.
            </p>
            <p>
                Includes desert exploration, guided archaeological tours, and accommodations in Zephyrion Sands' luxurious dune resorts.
            </p>
        </DestinationCard>
        <DestinationCard pricePerPerson="15000" travelTime="30 to 35" destination="Aquatica Vortex">
            <p>
                Aquatica Vortex is on an exoplanet with an aquatic environment, necessitating a longer warp journey to reach the destination.
            </p>
            <p>
                An underwater city on a watery exoplanet, perfect for marine enthusiasts.
            </p>
            <p>
                Includes a stay in the underwater city, marine excursions, and immersive aquatic experiences.
            </p>
        </DestinationCard>
        <DestinationCard pricePerPerson="20000" travelTime="40 to 45" destination="Zenithari Nexus">
            <p>
                The Zenithari Nexus is positioned deeper within space, requiring a longer warp jump to access the energy vortex where it's located.
            </p>
            <p>
                A space station at the heart of the Zenithari energy vortex, offering unique metaphysical experiences.
            </p>
            <p>
                Includes access to the Zenithari Nexus space station, metaphysical workshops, and spiritual journeys.
            </p>
        </DestinationCard>
    </div>
</Section>