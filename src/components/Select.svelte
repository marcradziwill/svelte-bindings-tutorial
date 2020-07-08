<script>
  let scoops = 1;
  let flavours = ["Mint choc chip"];

  let valuesOfHappyness = ["Happy", "Curious", "Excited"];

  function join(flavours) {
    if (flavours.length === 1) return flavours[0];
    return `${flavours.slice(0, -1).join(", ")} and ${
      flavours[flavours.length - 1]
    }`;
  }
</script>

<h2>Flavours</h2>

<select multiple bind:value={flavours}>
  {#each valuesOfHappyness as flavour}
    <option value={flavour}>{flavour}</option>
  {/each}
</select>

{#if flavours.length === 0}
  <p>Please select at least one value</p>
{:else}
  <p>You selected {join(flavours)}</p>
{/if}
