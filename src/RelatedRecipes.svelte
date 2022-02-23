<script>
  import RecipeCard from "./RecipeCard.svelte";
  import { related } from "./data/related";
</script>

<section class="component">
  <h2>Read more</h2>
  {#each related as dish, i (i)}
    <RecipeCard {dish} {i} />
  {/each}
</section>

<style>
  section {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 2rem;
    margin: 2rem;
  }
  h2 {
    text-align: center;
    grid-column: 1/-1;
    border: 1px solid var(--color-grey-500);
    border-width: 1px 0;
    padding: 1rem;
  }
</style>
