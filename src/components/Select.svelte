<script>
  let scoops = 1;
  let happyness = ["Happy"];

  let valuesOfHappyness = ["Happy", "Curious", "Excited"];

  function join(happyness) {
    if (happyness.length === 1) return happyness[0];
    return `${happyness.slice(0, -1).join(", ")} and ${
      happyness[flavours.length - 1]
    }`;
  }
</script>

<h2>Happyness</h2>

<select multiple bind:value={happyness}>
  {#each valuesOfHappyness as flavour}
    <option value={flavour}>{flavour}</option>
  {/each}
</select>

{#if happyness.length === 0}
  <p>Please select at least one value</p>
{:else}
  <p>You selected {join(happyness)}</p>
{/if}
