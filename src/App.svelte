
<script>


	let count = 0;

	function increment() {
		count += 1;
	}

  //import app.svelte from comp.svelte
  let test = '5';
</script>
<comp {test} />

<main>
  
<button on:click={increment}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>


  <div class="machine">
  <div>
    
  </div>

  <div>
  321
  </div>

  <div>
  321
  </div>

</div>

</main>

<style>
  .machine {
    display: flex;
    flex-wrap: wrap; /* Позволяет элементам переноситься на следующую строку, если они не помещаются */
  }

  .machine div {
    display: inline-block;
    width: 33%;
    box-sizing: border-box; /* Учитывает padding и border в ширине элемента */
  }
</style>



