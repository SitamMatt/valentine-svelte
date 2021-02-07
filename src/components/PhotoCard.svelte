<script lang="ts">
	export let src = "";
</script>

<div class="photo-container">
	<img {src} alt="hello sylwia" />
	<!-- <div class="elo" /> -->
</div>

<style>
	.elo {
		width: 100%;
		height: 100%;
		background-color: green;
		border: 10px solid white;
	}
	.photo-container {
	}
	.photo-container > img {
		border: 5px solid white;
		padding: 0;
		box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
		margin: auto;
		/* object-fit: cover; */
		max-width: 400px;
		max-height: 100%;
		background-color: white;
	}
</style>
