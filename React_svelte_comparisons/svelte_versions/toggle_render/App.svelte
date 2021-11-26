<script>

	let displayToggle = true;
	
  	const toggleDisplay = () => {
	  displayToggle = !displayToggle;
	}

</script>
	
<button on:click={toggleDisplay}>Toggle Display</button>
<br />
{#if displayToggle}
  <h1>Displayed!</h1>  
{/if}
