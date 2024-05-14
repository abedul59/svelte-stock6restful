<script>



function handleSubmit() {

  name3 = name2; 

  result2 = `https://stock6-restfulex.onrender.com/api/Stock6Sign202402/getstockinfo/${name3}`

  console.log(`最新得到網址為${result2}`)
  fetch(result2)
    .then((data) => data.json())
    .then((response) => {
      const { cStockName, cNewestSeason, cStockID } = response

	  tStockID = cStockID;
      
	  tStockName = cStockName;

	  tNewestSeason = cNewestSeason;


	  
      tStock6data2 = response;
      console.log(response)

      console.log(tStockName)
      console.log(tNewestSeason)
      console.log(tStockID)

    })
}
	export let tStockName, tNewestSeason, tStock6data2;
	export let name3;
	export let result2;
	export let tStockID;


</script>

<main>

	<input bind:value={name2} placeholder="輸入股票代碼" />
	<p>Hello {name2 || 'stranger'}!</p>
	<button on:click={handleSubmit}> Submit </button>
	<p>Hello1 {result2}</p> 
	<br>
	<p>Hello2 {tStockName2}</p>
	<br>
	<p>Hello3 {tNewestSeason2}</p>
	<br>
	<p>Hello4 {tStockID}</p>

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>