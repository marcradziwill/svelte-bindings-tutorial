<script>
  let value = `Checkout your textarea value with two-way data binding`;
</script>

<style>
  textarea {
    width: 100%;
    height: 200px;
  }
</style>

<textarea bind:value />

{@html value}
