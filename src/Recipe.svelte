<script>
  import Instructions from "./Instructions.svelte";
  import Reviews from "./Reviews.svelte";
  import AvgRating from "./AvgRating.svelte";
</script>

<article class="component">
  <section>
    <h2>Black-Eyed Pea Salad With Hot Sauce Vinaigrette</h2>
    <p class="issue">June 2020 Issue</p>
    <p class="author">By Carla Hall</p>
    <p class="date">June 17, 2020</p>
    <AvgRating />
  </section>
  <section>
    <img src="BlackEyedPeaSalad.webp" alt="" />
  </section>
  <section>
    <Instructions />
  </section>
  <section>
    <Reviews />
  </section>
</article>

<style>
  article {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  h2 {
    font-size: 3rem;
    line-height: 3rem;
  }
  section:first-child {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 90vh;
  }
  .date {
    order: -1;
  }
  section:first-child > * {
    max-width: 16ch;
    margin-left: auto;
    margin-right: auto;
  }
  section:not(:first-child, :nth-child(2)) {
    grid-column: 1/-1;
  }
  img {
    object-fit: cover;
    width: 100%;
    height: 100%;
  }
  @media only screen and (max-width: 600px) {
    article {
      grid-template-columns: 1fr;
    }
  }
</style>
