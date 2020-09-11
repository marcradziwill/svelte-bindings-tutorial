<script>
  let w;
  let h;
  let color = "green";
</script>

<style>
  input {
    display: block;
  }
  div {
    display: inline-block;
  }
  span {
    word-break: break-all;
  }
</style>

<input type="text" bind:value={color} />

<div bind:clientWidth={w} bind:clientHeight={h}>
  <span style="color: {color};">Let's change my color</span>
</div>
