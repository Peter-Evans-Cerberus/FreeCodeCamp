<script>

	let userInput = '';
	let toDoList = [];

	const handleSubmit = () => {
		toDoList = userInput.split(',');
	}

</script>
	
<!--HTML markup-->
<textarea
	bind:value={userInput}
	placeholder="Separate items with commas"
/>
<button on:click={handleSubmit}>Create List</button>
<h1>My "To Do" List: </h1>
<ul>
	{#each toDoList as item}
	<li>{item}</li>
	{/each}
</ul>
<!--End of HTML markup-->


<style>
	textarea {
		width: 235;
		margin: 5;
	}
</style>