<script lang="ts">
	import MainSection from "./MainSection.svelte";

	import Section from "./Section.svelte";
</script>

<main>
	<div class="bg-red-400">
		<MainSection />
		<!-- <Section onScreen={true} /> -->
		<!-- <Section watch={true} /> -->
		<!-- <Section watch={true} /> -->
	</div>
</main>

<style global lang="postcss">
	/* only apply purgecss on utilities, per Tailwind docs */
	/* purgecss start ignore */
	@tailwind base;
	@tailwind components;
	@tailwind utilities;
	.wrapper {
		background-color: rgba(239, 68, 68, var(--tw-bg-opacity));
	}
	/* purgecss end ignore */
</style>
