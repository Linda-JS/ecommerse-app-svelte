<script>
  import { onMount, onDestroy } from "svelte";
  import products from "../../stores/defaultProducts";
  import Product from "./Product.svelte";
  export let title;

  //// let unsubscribe;
  // onMount(() => {
  //   unsubscribe = products.subscribe((value) => {
  //     localProducts = value;
  //   });
  // });
  // onDestroy(() => {
  //   unsubscribe();
  // });
</script>

<section class="section">
  <h2 class="section-title">{title}</h2>
  <div class="products-center">
    {#each $products as product (product.id)}
      <Product {product} />
    {/each}
  </div>
</section>
