
<script>
	let input;
	let submit;
	
	function handleSubmit(){
		submit = input;
	}
	
	</script>
	
	<main>
		<form on:submit|preventDefault={handleSubmit}}>
			<input bind:value={input}/>
			<button type="submit"></button>
		</form>
		<h1>{submit}</h1>
		
	</main>