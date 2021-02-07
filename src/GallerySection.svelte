<script lang="ts">
	import PhotoCard from "./components/PhotoCard.svelte";
	import { photos } from "./photo-datasource";
</script>

<section
	class="grid grid-flow-col grid-cols-3 grid-rows-2 gap-5 p-10 h-full w-full"
>
	{#each photos as photo}
		<PhotoCard src={photo} />
	{/each}
</section>
