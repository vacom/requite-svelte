<script>
  import Error from "./Error.svelte";

  export let data = [];
  export let components = {};
</script>

{#each data as item}
  <svelte:component this={components[item.name] || Error}  {...item.props} />
{/each}
