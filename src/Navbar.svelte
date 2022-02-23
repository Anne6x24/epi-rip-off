<script>
  function toggle() {
    document.body.classList.toggle("highlight");
  }
</script>

<nav class="component">
  <h1>Epicurious</h1>
  <a href="#/">Recipes &amp; Menus</a>
  <a href="#/">Expert Advice</a>
  <a href="#/">Ingredients</a>
  <a href="#/">Holidays &amp; Events</a>
  <div>
    <a href="#/">Sign In</a>
    <a href="#/">Subscribe</a>
    <button on:click={toggle}>Draw outlines</button>
  </div>
</nav>

<style>
  h1 {
    text-transform: lowercase;
    color: red;
    font-size: 1.5rem;
  }
  nav {
    display: flex;
    align-items: baseline;
    gap: 1rem;
    padding: 0 1rem;
    border-bottom: 1px solid #000;
  }
  a {
    text-decoration: none;
    color: var(--color-grey-250);
    transition: all 0.2s;
    font-size: 0.8rem;
  }
  button {
    display: inline;
    margin-top: 0;
    width: auto;
  }
  a:hover {
    color: red;
    text-decoration: underline;
  }
  div {
    margin-left: auto;
  }
</style>
