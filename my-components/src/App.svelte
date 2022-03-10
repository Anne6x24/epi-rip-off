<script>
	import "carbon-components-svelte/css/white.css";
	import { Button } from "carbon-components-svelte";
	import { MultiSelect } from "carbon-components-svelte";
	import { Slider } from "carbon-components-svelte";
</script>

<Button>Primary button</Button>

<MultiSelect
  titleText="Contact"
  label="Select contact methods..."
  items={[
    { id: "0", text: "Slack" },
    { id: "1", text: "Email" },
    { id: "2", text: "Fax" },
  ]}
/>

<Slider />