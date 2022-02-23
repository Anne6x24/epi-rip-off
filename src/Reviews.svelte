<script>
  import Review from "./Review.svelte";
  import { reviews } from "./data/reviews";
</script>

<div class="wrapper component">
  <h3>Leave a Review</h3>

  <form>
    <textarea />
  </form>

  <h3>Reviews ({reviews.length})</h3>
  <ul>
    {#each reviews as review, i (i)}
      <Review {...review} />
    {/each}
  </ul>
</div>

<style>
  ul {
    list-style-type: none;
    padding: 0;
  }
</style>
