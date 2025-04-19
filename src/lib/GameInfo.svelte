<script lang="ts">
	interface Props {
		gameName: string;
		gamePhoto: string;
		gameBlurb: string;
	}

	let { gameName, gamePhoto, gameBlurb }: Props = $props();
</script>

<div>
	<h1>{gameName}</h1>
	<img src={gamePhoto} alt="The image for {gamePhoto}" width="150" height="150" />
	<p>{gameBlurb}</p>
</div>

<style>
	h1 {
		color: white;
	}

	p {
		color: white;
	}
</style>
