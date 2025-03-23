<script lang="ts">
  interface Props {
    playerName : string;
    playerPhoto: string;
    playerBlurb: string;
  }

  let {playerName, playerPhoto, playerBlurb}: Props = $props();
</script>

<div>
  <h1>{playerName}</h1>
  <img src={playerPhoto} alt="The image for {playerName}" width="150" height="150"/>
  <p>{playerBlurb}</p>
</div>
