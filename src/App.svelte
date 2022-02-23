<script>
  import Navbar from "./Navbar.svelte";
  import Recipe from "./Recipe.svelte";
</script>

<Navbar />
<Recipe />

<footer>
  <p>
    <a
      href="https://www.epicurious.com/recipes/food/views/black-eyed-pea-salad-with-hot-sauce-vinaigrette"
      >https://www.epicurious.com/recipes/food/views/black-eyed-pea-salad-with-hot-sauce-vinaigrette</a
    >
  </p>
</footer>

<style>
  footer {
    background: black;
  }
  p {
    max-width: none;
    padding: 1rem;
  }
  a {
    color: white;
  }
</style>
