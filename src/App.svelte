<script>
  import { Router, Route, Link } from "svelte-routing";
  import Navbar from "./route/layout/navbar.svelte";
  import Home from "./route/home.svelte";
  import Page1 from "./route/taliwind.svelte";
  export let url = "";
</script>

<Navbar />
<Router url="{url}">
<Route path="/" ><Home /></Route>
<Route path="page1" ><Page1 /></Route>
</Router>
