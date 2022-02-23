<script>
  export let dish;
  export let i;
</script>

<article>
  <img src={`https://picsum.photos/id/${i}/400/400`} alt="" />
  <h3>{dish.name}</h3>
  <p>{dish.desc}</p>
</article>

<style>
  h3::after {
    display: block;
    content: "";
    padding-bottom: 1rem;
  }
  h3::after {
    border-bottom: 1px solid rgb(51, 51, 51);
    margin-bottom: 1rem;
    width: 5rem;
  }
</style>
