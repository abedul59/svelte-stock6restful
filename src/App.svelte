<script>



function handleSubmit() {

  name3 = [...name3, name2]; //解壓縮空陣列name3 帶入輸入的name2 全新陣列 位址有變 才會響應

  result2 = `https://stock6-restfulex.onrender.com/api/Stock6Sign202402/getstockinfo/${name3}`

  name3 = [];//clean name3 array to avoid repitition
  console.log(`最新得到網址為${result2}`)
  fetch(result2)
    .then((data) => data.json())
    .then((response) => {
      const { cStockName, cNewestSeason } = response
      
	  tStockName = [...tStockName, cStockName];

	  tNewestSeason = [...tNewestSeason, cNewestSeason];
	  
      let tStock6data2 = response;
      console.log(response)

      console.log(tStockName)
      console.log(tNewestSeason)
      console.log(tStock6data2)
    })
}
	export let tStockName = [], tNewestSeason = [], tStock6data2;
	
	export let name2;
	export let name3 = [];
	export let result2;


</script>

<main>

	<input bind:value={name2} placeholder="輸入股票代碼" />
	<p>Hello {name2 || 'stranger'}!</p>
	<button on:click={handleSubmit}> Submit </button>
	<p>Hello1 {result2}</p> 
	<br>
	<p>Hello2 {tStockName}</p>
	<br>
	<p>Hello3 {tNewestSeason}</p>
	<br>
	<p>Hello4 {tStock6data2}</p>

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