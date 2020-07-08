<script>
  let showMeMyAwesomeGif = false;
</script>

<label>
  <input type="checkbox" bind:checked={showMeMyAwesomeGif} />
  Yes, show me my GIF
</label>

{#if showMeMyAwesomeGif}
  <iframe
    src="https://giphy.com/embed/Z6f7vzq3iP6Mw"
    width="480"
    height="203"
    frameBorder="0"
    class="giphy-embed"
    allowFullScreen />
  <p>
    <a href="https://giphy.com/gifs/awesome-yes-old-school-Z6f7vzq3iP6Mw">
      via GIPHY
    </a>
  </p>
{:else}
  <p>Nooooo awesome GIF here</p>
{/if}
