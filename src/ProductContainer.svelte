<script lang="ts">
  import ProductCard from './ProductCard.svelte';

  const products = [
    {
      name: 'Rose Noir',
      image: '../mob_rosenoir_edp-100_c_1.jpeg',
      description: 'Rose Noir',
    },
    {
      name: 'Bal D Afrique',
      image: '../mob_baldafrique_edp-100_d_1.jpeg',
      description: 'Bal D Afrique',
    },
    {
      name: 'Blanche',
      image: '../mob_blanche_edp-100_d.jpeg',
      description: 'Blanche',
    },
    {
      name: 'Sundazed',
      image: '../mob_sundazed_edp-100_a.jpeg',
      description: 'Sundazed',
    },
  ];
</script>

<div class="product-list">
  {#each products as product (product.name)}
    <ProductCard {product} />
  {/each}
</div>

<style>
  .product-list {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    margin-top: 2.5rem;
    max-width: 100%;
    overflow: hidden;
    padding: 0 1.5rem;
    border: solid 0.025rem #000000;
  }

  /* Media query for mobile screens */
  @media (max-width: 768px) {
    .product-list {
      flex-direction: column;
      padding-left: 0.938rem;
      padding-right: 0.938rem;
      margin-top: 2rem;
    }
  }
</style>
