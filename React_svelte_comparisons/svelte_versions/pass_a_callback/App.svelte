<script>
	let name="MyApp";
	import GetInput from "./GetInput.svelte";
	import RenderInput from "./RenderInput.svelte";
	
	let input = '';

	function handleChange(event) {
		input = event.target.value;
	}
</script>
	
<GetInput bind:input />
<RenderInput input={input}/>