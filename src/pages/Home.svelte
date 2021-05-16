<script>
  import Hero from "../components/Hero.svelte";
  import { link } from "svelte-routing";
  //Featured Products
</script>

<Hero>
  <a href="/products" class="btn btn-primary btn-hero" use:link>shop now</a>
</Hero>
