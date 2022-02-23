<script>
  let expanded = true;
</script>

<footer class:expanded>
  <div>
    <button on:click={() => (expanded = !expanded)}>
      {#if !expanded}
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-chevron-up"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M7.646 4.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1-.708.708L8 5.707l-5.646 5.647a.5.5 0 0 1-.708-.708l6-6z"
          />
        </svg>
      {:else}
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="16"
          height="16"
          fill="currentColor"
          class="bi bi-chevron-down"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z"
          />
        </svg>
      {/if}
    </button>
    <p>
      <a
        href="https://www.epicurious.com/recipes/food/views/black-eyed-pea-salad-with-hot-sauce-vinaigrette"
        >https://www.epicurious.com/recipes/food/views/black-eyed-pea-salad-with-hot-sauce-vinaigrette</a
      >
    </p>
  </div>
</footer>

<style>
  footer {
    background: black;
    position: fixed;
    bottom: 0;
    width: 100%;
    transition: all 0.3s;
    height: 80px;
  }
  .expanded {
    height: 320px;
  }
  button {
    all: unset;
    cursor: pointer;
    width: auto;
    position: absolute;
    right: 1rem;
  }
  button svg {
    fill: white;
  }
  p {
    max-width: none;
    padding: 1rem;
  }
  a {
    color: white;
  }
</style>
