<script>
  let todos = [
    { done: false, text: "Olives" },
    { done: false, text: "Goat cheese" },
    { done: false, text: "Wine" }
  ];
</script>

<h1>Todos</h1>

{#each todos as todo}
  <div class:done={todo.done}>
    <input type="checkbox" bind:checked={todo.done} />

    <input placeholder="What needs to be done?" bind:value={todo.text} />
  </div>
{/each}
{JSON.stringify(todos)}
