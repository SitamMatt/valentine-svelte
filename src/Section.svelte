<script lang="ts">
	import { fade, fly } from "svelte/transition";

	let y;
	$: if (y) {
		if (el != null && watch) {
			let height = el.scrollHeight;
			let top = el.getBoundingClientRect().top;
			if (top <= 0 && !onScreen) {
				console.log(height + " " + top);
				console.log("fade-in");
				onScreen = true;
			}
		}
	}
	let el: Element;
	export let onScreen: boolean = false;
	export let watch: boolean;
</script>

<svelte:window bind:scrollY={y} />

<main class="h-screen flex" bind:this={el}>
	<img
		src="heart.png"
		class="m-auto"
		class:fade-in={onScreen}
		class:hidden={!onScreen}
		alt="alternatywne serduszko <3"
	/>
	<!-- <h1>Hello {y} {iy} {t?.getBoundingClientRect().top}</h1> -->
</main>

<style>
	.fade-in {
		animation: fadein 1s;
		animation-fill-mode: forwards;
	}

	@keyframes fadein {
		from {
			opacity: 0;
			transform: translate3d(-10%, 0, 0);
		}

		to {
			opacity: 1;
			transform: none;
		}
	}
</style>
