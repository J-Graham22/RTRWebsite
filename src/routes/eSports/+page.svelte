<script>
	import PlayerProfile from "$lib/PlayerProfile.svelte";

  import Punx from "$lib/assets/yu.png"
  import Basket from "$lib/assets/basket.jpg"
  import Daydream from "$lib/assets/daydream.jpg"
</script>

<div>
  <h1>Remember the Ravens</h1>
  <h1>esports</h1>

  <PlayerProfile
    playerName = {"PUNX"}
    playerPhoto = {Punx}
    playerBlurb = {"He's a super guy!!"}
  />
  <PlayerProfile
    playerName = {"Daydream"}
    playerPhoto = {Daydream}
    playerBlurb = {"He plays 'em all!!"}
  />
  <PlayerProfile
    playerName = {"Basket"}
    playerPhoto = {Basket}
    playerBlurb = {"RUNESCAPE??!!"}
  />
</div>
