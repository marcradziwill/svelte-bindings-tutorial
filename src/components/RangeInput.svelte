<script>
  let counter = 1;
</script>

<input type="range" bind:value={counter} min="0" max="10" />
<p>{counter}</p>
