<script>
	import { Router, Link, Route } from "svelte-routing";
	import Stock6Sign2403 from "./routes/Stock6Sign2403.svelte";

  
	export let url = "";
  </script>
  
  <Router {url}>
	<nav>
	  <Link to="/">Home</Link>
	  <Link to="/Stock6Sign2403">Stock6Sign2403</Link>

	</nav>
	<div>
	  <Route path="/Stock6Sign2403" component={Stock6Sign2403} />


	</div>
  </Router>