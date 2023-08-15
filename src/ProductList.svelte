<script lang="ts">
  import ProductCard from './ProductCard.svelte';

  const products = [
    {
      name: 'Rose Noir',
      category: 'Perfume',
      image: '../mob_rosenoir_edp-100_c_1.jpeg',
      price: 1500,
      volume: '100 ml',
      description:
        'The fresh bitters of lime, elegance of bergamot, and calmness of cedarwood coexist and deliver a moment of refresh.',
    },
    {
      name: 'Bal D Afrique',
      category: 'Perfume',
      image: '../mob_baldafrique_edp-100_d_1.jpeg',
      price: 1500,
      volume: '100 ml',
      description:
        'Epicene beauty blended with warmth of sweet suede, calming cedarwood, vanilla, and musk.',
    },
    {
      name: 'Blanche',
      category: 'Perfume',
      image: '../mob_blanche_edp-100_d.jpeg',
      price: 1500,
      volume: '100 ml',
      description:
        'Serene and languid moments culminated by a harmony of vetiver, sandalwood, and fresh cardamom.',
    },
    {
      name: 'Sundazed',
      category: 'Perfume',
      image: '../mob_sundazed_edp-100_a.jpeg',
      price: 1500,
      volume: '100 ml',
      description:
        'A remembrance of the purest seasons through fresh, yet warm scents of neroli and orange blossom.',
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
    padding: 0 49.375rem;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .product-list {
      padding: 0 29.375rem;
    }
  }

  /* Media queries for standard desktop screens */
  @media (max-width: 1920px) {
    .product-list {
      padding: 0 1.5rem;
    }
  }

  /* Media query for mobile screens */
  @media (max-width: 640px) {
    .product-list {
      flex-direction: column;
      padding: 0 0.938rem;
      margin-top: 2rem;
    }
  }
</style>
