<script>


let name2;
let result2 = '';

function handleSubmit() {



  let result2 = `https://stock6-restfulex.onrender.com/api/Stock6Sign202403/getstockinfo/${name2}`

  console.log(`最新得到網址為${result2}`)
  fetch(result2)
    .then((data) => data.json())
    .then((response) => {
      const { cStockName, cNewestSeason } = response
      let tStockName = cStockName
      let tNewestSeason = cNewestSeason
      let tStock6data2 = response

      console.log(response)

      console.log(tStockName)
      console.log(tNewestSeason)
      console.log(tStock6data2)
    })
}
	export let tStockName, tNewestSeason, tStock6data2;
	export let name;


</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
	<br>
	<input bind:value={name2} placeholder="enter your name" />
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