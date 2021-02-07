<script lang="ts">
	import FullscreenWrapper from "./components/FullscreenWrapper.svelte";

	import GallerySection from "./GallerySection.svelte";

	import MainSection from "./MainSection.svelte";

	import Section from "./Section.svelte";
</script>

<main>
	<div class="bg-red-300">
		<FullscreenWrapper>
			<MainSection />
		</FullscreenWrapper>
		<FullscreenWrapper>
			<GallerySection />
		</FullscreenWrapper>
	</div>
</main>

<style global lang="postcss">
	/* only apply purgecss on utilities, per Tailwind docs */
	/* purgecss start ignore */
	@tailwind base;
	@tailwind components;
	@tailwind utilities;
	/* purgecss end ignore */
</style>
