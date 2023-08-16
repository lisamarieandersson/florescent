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

<div class="product-container">
  <div class="product-header">
    <h2>Discover our products</h2>
  </div>
  <div class="product-list">
    {#each products as product (product.name)}
      <ProductCard {product} />
    {/each}
  </div>
</div>

<style>
  .product-container {
    padding: 0 49.375rem;
    text-align: center;
    margin-bottom: 4rem;
  }

  .product-header {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 5rem;
  }

  .product-list {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    max-width: 100%;
    overflow: hidden;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .product-container {
      padding: 0 29.375rem;
    }
  }

  /* Media queries for standard desktop screens */
  @media (max-width: 1920px) {
    .product-container {
      padding: 0 1.5rem;
    }
  }

  /* Media query for smaller desktop and tablet screens */
  @media (max-width: 1024px) {
    .product-container {
      margin-bottom: 2rem;
      text-align: center;
    }
  }

  /* Media query for mobile screens */
  @media (max-width: 640px) {
    .product-container {
      padding: 0 0.875rem;
    }

    .product-list {
      flex-direction: column;
    }
  }
</style>
