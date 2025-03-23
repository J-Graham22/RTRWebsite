<script lang="ts">
  let artistName: string = "";
  let artistPhoto: string = "";
  let artistBlurb: string = "";
</script>

<div>
  <h1>{artistName}</h1>
  <img src={artistPhoto} alt="The image for {artistName}"/>
  <p>{artistBlurb}</p>
</div>
