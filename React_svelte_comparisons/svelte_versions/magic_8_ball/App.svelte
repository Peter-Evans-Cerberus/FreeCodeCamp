<script>
  
	let userInput = '';
	let randomIndex;
	let answer = '';
	const possibleAnswers = [
      'It is certain',
      'It is decidedly so',
      'Without a doubt',
      'Yes, definitely',
      'You may rely on it',
      'As I see it, yes',
      'Outlook good',
      'Yes',
      'Signs point to yes',
      'Reply hazy try again',
      'Ask again later',
      'Better not tell you now',
      'Cannot predict now',
      'Concentrate and ask again',
      "Don't count on it",
      'My reply is no',
      'My sources say no',
      'Most likely',
      'Outlook not so good',
      'Very doubtful'
    ];

  function ask() {
  	if (userInput) {
	  	randomIndex = Math.floor(Math.random() * 20);
		  userInput = '';
		  answer = possibleAnswers[randomIndex];
	  }
  }

</script>
	
<input type="text" bind:value={userInput} />
<br />
<button on:click={ask}>Ask the Magic Eight Ball!</button>
<br />
<h3>Answer:</h3>
<p>{answer}</p>


<style>
	input {
		width: 235px;
		margin: 5px;
}
</style>