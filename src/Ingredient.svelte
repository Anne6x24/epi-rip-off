<script>
  export let base;
  export let multiplier;
  $: calculateAmount = (base) => {
    return parseFloat(((base / 4) * multiplier).toFixed(1));
  };
  let checked = false;
</script>

<li class:checked class="component">
  <label>
    <input type="checkbox" on:change={() => (checked = !checked)} />
    {#if base > 0}
      {calculateAmount(base)}
    {/if}
    <slot />
  </label>
</li>

<style>
  li {
    margin-bottom: 1.5rem;
  }
  .checked {
    text-decoration: line-through;
  }
</style>
