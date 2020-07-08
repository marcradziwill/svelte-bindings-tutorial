<script>
  import TextInput from "./components/TextInput.svelte";
  import NumberInput from "./components/NumberInput.svelte";
  import RangeInput from "./components/RangeInput.svelte";
  import Checkbox from "./components/Checkbox.svelte";
  import Group from "./components/Group.svelte";
  import Textarea from "./components/Textarea.svelte";
  import Select from "./components/Select.svelte";
  import ContentEditable from "./components/ContentEditable.svelte";
  import Loop from "./components/Loop.svelte";
</script>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <TextInput />
  <hr />
  <NumberInput />
  <hr />
  <RangeInput />
  <hr />
  <Checkbox />
  <hr />
  <Group />
  <hr />
  <Textarea />
  <hr />
  <Select />
  <hr />
  <ContentEditable />
  <hr />
  <Loop />
</main>
