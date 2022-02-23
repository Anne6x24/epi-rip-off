<script>
  import Rating from "./Rating.svelte";
  import Ingredient from "./Ingredient.svelte";

  let multiplier = 4;
</script>

<div class="wrapper component">
  <p>
    Black-eyed peas hold a special significance in the heart of every
    African-American. We eat them for good luck on New Year’s in a rice dish
    known as hoppin’ John. That tradition comes from a long history of
    black-eyed peas symbolizing luck and prosperity in Africa, where they’re
    part of spiritual ceremonies too. They’re a part of our culinary DNA. And
    they’re delicious.
  </p>

  <p>
    Black-eyed peas are tender, skin to center, and this helps them soak up
    sauces. Because they’re nice and mild, I drench them with a hot sauce
    dressing, honeyed yet sharp with garlic and mustard. In this salad,
    cucumbers and onion balance the peas’ creaminess with crunch, and tomatoes
    burst juiciness. Down South, we call this a sitting salad. It can sit on the
    summer picnic table without wilting, so it’s the perfect potluck dish. Get
    ready for this salad to become one of your favorites.
  </p>
  <h3>Ingredients</h3>
  <div class="serves">
    <button on:click={() => (multiplier -= 1)}> - </button>
    <p>{multiplier} servings</p>
    <button on:click={() => (multiplier += 1)}> + </button>
  </div>
  <ul>
    <Ingredient base={2} {multiplier}>
      garlic cloves, grated on a Microplane
    </Ingredient>
    <Ingredient base={2} {multiplier}>
      tablespoons apple cider vinegar
    </Ingredient>
    <Ingredient base={1} {multiplier}>tablespoon yellow mustard</Ingredient>
    <Ingredient base={1} {multiplier}>tablespoon hot sauce</Ingredient>
    <Ingredient base={1} {multiplier}>teaspoon honey</Ingredient>
    <Ingredient base={0} {multiplier}
      >Kosher salt and freshly ground black pepper</Ingredient
    >
    <Ingredient base={6} {multiplier}>tablespoons vegetable oil</Ingredient>
    <Ingredient base={1} {multiplier}>
      (15-ounce) can black-eyed peas, rinsed and drained
    </Ingredient>
    <Ingredient base={1} {multiplier}>
      mini cucumbers, cut into ½-inch dice
    </Ingredient>
    <Ingredient base={0.5} {multiplier}>sweet onion, finely chopped</Ingredient>
    <Ingredient base={1} {multiplier}>
      pint cherry tomatoes or grape tomatoes, halved
    </Ingredient>
    <Ingredient base={0.25} {multiplier}>cup picked fresh dill</Ingredient>
  </ul>

  <ol>
    <li>
      <strong>Step 1</strong>
      <p>
        Whisk the garlic, vinegar, mustard, hot sauce, honey, 1/4 teaspoon salt,
        and ¼ teaspoon pepper in a large bowl until smooth. While whisking, add
        the oil in a slow, steady stream. Whisk until emulsified.
      </p>
    </li>
    <li>
      <strong>Step 2</strong>
      <p>
        Add the peas, cucumbers, onion, tomatoes, dill, and 1/2 teaspoon salt.
        Toss until well mixed. You can serve this right away or let it sit at
        room temperature for up to 1 hour.
      </p>
    </li>
    <li>
      <strong>Step 3</strong>
      <p>DO AHEAD: The salad can be refrigerated for up to 1 day.</p>
    </li>
  </ol>
  <Rating />
</div>

<style>
  h3 {
    border-bottom: 1px solid var(--color-grey-250);
    padding-bottom: 1rem;
  }
  .serves {
    display: flex;
    gap: 1rem;
    justify-content: center;
    align-content: center;
    align-items: center;
  }
  .serves p {
    padding: 0;
    margin: 0;
  }
  button {
    width: 40px;
    height: 40px;
    margin-top: 0;
  }
  ol,
  ul {
    list-style-type: none;
  }
</style>
