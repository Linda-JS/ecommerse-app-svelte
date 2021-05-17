<script>
  //Pages
  import About from "./pages/About.svelte";
  import Checkout from "./pages/Checkout.svelte";
  import Home from "./pages/Home.svelte";
  import Login from "./pages/Login.svelte";
  import Products from "./pages/Products.svelte";
  import ProductTemplate from "./pages/ProductTemplate.svelte";
  import Navbar from "./components/Navbar/Navbar.svelte";
  //Router
  import { Router, Route, Link } from "svelte-routing";
</script>

<Router>
  <Navbar />
  <Route path="/" component={Home} />
  <Route path="/about" component={About} />
  <Route path="/login" component={Login} />
  <Route path="/products" component={Products} />
  <Route path="/products/:id" component={ProductTemplate} />
</Router>
