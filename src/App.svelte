<script lang="ts">
	import JsonExample from "./JsonExample.svelte";

	const components = {
		json: JsonExample,
	}

	const current = components.json;
</script>

<main>
	<div class="padding">
		<svelte:component this={current}/>
	</div>
	<div class="bottom-space"></div>
</main>

<style>
	.padding {
		padding: 20px;
		padding-bottom: 50px;
	}
	main {
		position: relative;
		width: 100%;
		height: 100%;
		overflow: scroll;
	}
</style>