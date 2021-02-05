<script lang="ts">
</script>

<section class="h-screen flex p-8">
	<img src="heart.png" class="m-auto fade-in" alt="alternatywne serduszko <3" />
</section>

<style>
	.fade-in {
		animation: fadein 1.5s;
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
