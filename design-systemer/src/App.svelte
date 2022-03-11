<script>
	import Button from "./Button.svelte"
	import Badge from "./Badge.svelte"
	import Cards from "./Cards.svelte"
	import Footer from "./Footer.svelte"
	import Inbox from "./Inbox.svelte"

</script>

<main>
	<section class="main_section">

<h1>Anne og Katjas første components</h1>

<!-- badge -->
<section class="padding_section">

	<h2>Badge component</h2>

	<article class="badge_section">
	<Badge>neutral</Badge>
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Badge>neutral</Badge>'}</code></pre>
	</article>

	<article class="badge_section">
	<Badge type="primary">primary</Badge>
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Badge type="primary">primary</Badge>'}</code></pre>	
	</article>

	<article class="badge_section">
	<Badge type="secondary">secondary</Badge>
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Badge type="secondary">secondary</Badge>'}</code></pre>
	</article>

	<article class="badge_section">
	<Badge type="accent">accent</Badge>
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Badge type="accent">accent</Badge>'}</code></pre>
	</article>

	<article class="badge_section">
	<Badge type="ghost">ghost</Badge>
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Badge type="ghost">ghost</Badge>'}</code></pre>
	</article>

</section>



<!-- button -->
<section class="padding_section">

	<h2>Button component</h2>

	<article class="button_section">
	<Button>BUTTON</Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button>BUTTON</Button>'}</code></pre>
	</article>

	<article class="button_section">
	<Button type="primary">PRIMARY</Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button type="primary">PRIMARY</Button>'}</code></pre>	
	</article>

	<article class="button_section">
	<Button type="secondary">SECONDARY</Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button type="secondary">SECONDARY</Button>'}</code></pre>
	</article>

	<article class="button_section">
	<Button type="accent">ACCENT</Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button type="secondary">SECONDARY</Button>'}</code></pre>
	</article>

	<article class="button_section">
	<Button type="ghost">GHOST</Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button type="ghost">GHOST</Button>'}</code></pre>
	</article>

	<article class="button_section">
	<Button type="link"><a href="link">LINK</a></Button>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Button type="ghost">GHOST</Button>'}</code></pre>
	</article>

	

</section>



<!-- card -->
	<section class="padding_section">

	<h2>Card component</h2>

	<article class="card_section">
	<Cards></Cards>

	<div class="kode_code">
	<img src="./QuillArrowRight.svg" alt="">
	<pre><code>{'<Cards></Cards>'}</code></pre>
	</div>

	</article>

	</section>


<!-- Button w Badge component -->
	<section class="hej padding_section">

	<h2>Button w Badge component</h2>

	<article class="inbox_section">
	<Inbox></Inbox>
	<img src="./QuillArrowRight.svg" alt="">
	<pre class="fit_content"><code>{'<Inbox></Inbox>'}</code></pre>
	</article>

	</section>


</section>
</main>

<!-- Footer component -->
	<section>

	<h2>Footer component</h2>

	<article class="footer_section">
	<Footer></Footer>
	<pre><code>{'<Footer></Footer>'}</code></pre>
	</article>

	</section>




	<style>
		
		.badge_section,
		.button_section,
		.inbox_section,
		.card_section
		 {
			display: flex;
			gap: 3rem;
		}

		.kode_code {
			display: flex;
			height: fit-content;
			padding-top: 15rem;
			gap: 3rem;
		}

		pre {
			padding: 0.5rem 1rem;
			border-radius: 0.4rem;
			color: white;
			background-color: black;
			width: fit-content;
		}

		main {
			display: grid;
			grid-template-columns: 1fr 2fr 1fr;
		}

		.main_section {
			grid-column: 2/3;
		}

		.fit_content {
			height: fit-content;
		}

		.padding_section {
			margin-top: 4rem;
		}

	</style>




