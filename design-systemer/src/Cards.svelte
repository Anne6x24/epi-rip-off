
<script>
    import Button from "./Button.svelte"
    import Badge from "./Badge.svelte"
</script>


<section class="card">
<img src="./stolthed.png" alt="">
<div class="flex">
<h3>Shoes! <Badge type="secondary">NEW</Badge></h3>

</div>
<p>If a dog chewes shoes whoes shoes does he choose?</p>
<Badge type="ghost_border">Fashion</Badge>
<Badge type="ghost_border">Products</Badge>
<div class="blue">
<Button type="primary">BUY NOW</Button>
</div>
</section>

<style>
   .card {
       width: 25rem;
       border-radius: 10px 10px 10px 10px;
       box-shadow: 2px 10px darkgrey;
       
       
   }
   
   img {
       max-width: 25rem;
       border-radius: 15px 15px 0px 0px;
   }
   .flex {
       display: flex;
   }

   h3 {
       margin-right: 1rem;
   }

   .blue {
       margin-left: 19rem;
   }

   

</style>

