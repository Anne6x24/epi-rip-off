<script>
	import Button from "./Button.svelte"
	import Badge from "./Badge.svelte"
	import Cards from "./Cards.svelte"
	import Footer from "./Footer.svelte"
	import Inbox from "./Inbox.svelte"

</script>

<Badge>neutral</Badge>
<Badge type="primary">primary</Badge>
<Badge  type="secondary">secondary</Badge>
<Badge  type="accent">accent</Badge>
<Badge  type="ghost">ghost</Badge>





<section>
<Button>BUTTON</Button>
<Button type="primary">PRIMARY</Button>
<Button type="secondary">SECONDARY</Button>
<Button type="accent">ACCENT</Button>
<Button type="ghost">GHOST</Button>
<Button type="link"><a href="link">LINK</a></Button>
</section>


<section>
	<Cards></Cards>
	</section>



	<section class="hej">
		<Inbox></Inbox>
	</section>



<Footer></Footer>





