<script>
  export let review;
  export let name;
  export let city;
  export let date;
</script>

<li class="component">
  <p>{review}</p>
  <div>{name} - {city} - {date}</div>
</li>

<style>
  li {
    border-bottom: 1px solid var(--color-grey-700);
  }
  div {
    padding-bottom: 1rem;
    text-transform: uppercase;
    color: var(--color-grey-500);
    font-weight: 300;
  }
</style>
