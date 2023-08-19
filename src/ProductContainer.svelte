<script lang="ts">
  import ProductCard from './ProductCard.svelte';

  const products = [
    {
      name: 'Enchanted April',
      category: 'Perfume',
      image: '../enchanted-april.png',
      price: 1500,
      volume: '100 ml',
      description:
        'The fresh bitters of lime, elegance of bergamot, and calmness of cedarwood coexist and deliver a moment of refresh.',
    },
    {
      name: 'Atlas Moon',
      category: 'Perfume',
      image: '../atlas-moon.png',
      price: 1500,
      volume: '100 ml',
      description:
        'Epicene beauty blended with warmth of sweet suede, calming cedarwood, vanilla, and musk.',
    },
    {
      name: 'Iris Haze',
      category: 'Perfume',
      image: '../iris-haze.png',
      price: 1500,
      volume: '100 ml',
      description:
        'Serene and languid moments culminated by a harmony of iris, vetiver, sandalwood, and fresh cardamom.',
    },
    {
      name: 'Peony Whispers',
      category: 'Perfume',
      image: '../peony-whispers.png',
      price: 1500,
      volume: '100 ml',
      description:
        'A remembrance of the purest seasons through fresh, yet warm scents of peony, neroli and orange blossom.',
    },
  ];
</script>

<div class="product-container">
  <div class="product-header">
    <h2>Shop our latest products</h2>
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

  h2 {
    font-weight: 400;
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
