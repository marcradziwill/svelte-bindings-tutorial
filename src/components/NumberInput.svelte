<script>
  let counter = 1;
</script>

<input type="number" bind:value={counter} min="0" max="10" />
<p>{counter}</p>
