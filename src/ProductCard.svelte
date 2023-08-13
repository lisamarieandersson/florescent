<script lang="ts">
  export let product: {
    name: string;
    category: string;
    image: string;
    price: number;
    volume: string;
    description: string;
  };
</script>

<div class="product-card">
  <img src={product.image} alt={product.name} />
  <h3 class="product-name">{product.name}</h3>
  <h4 class="product-category">{product.category}</h4>
  <div class="volume-and-price">
    <h4>{product.volume}</h4>
    <h4>{product.price} SEK</h4>
  </div>
  <div class="line" />
  <p class="description">{product.description}</p>
  <p class="read-more">Read more</p>
  <button>Add to Cart</button>
</div>

<style>
  .product-card {
    text-align: center;
    padding: 0 0.625rem;
    max-width: calc(25% - 0.025rem);
    box-sizing: border-box;
  }

  .product-name {
    text-transform: uppercase;
    font-weight: 400;
    margin-bottom: 0.125rem;
  }

  h4 {
    margin-top: 0.25rem;
    margin-bottom: 0.75rem;
  }

  img {
    max-width: 100%;
    height: auto;
  }

  .volume-and-price {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .description {
    height: 9.2rem;
  }

  .line {
    height: 0.025rem;
    background: #000000;
  }

  p {
    font-size: 0.875rem;
    text-align: left;
  }

  .read-more {
    font-weight: 400;
  }

  button {
    border-radius: 0;
    font-family: 'Fraunces', serif;
    font-weight: 300;
    background: #ffffff;
    border: solid 0.025rem #000000;
    padding: 1rem;
    text-transform: uppercase;
    width: 100%;
    text-align: center;
  }

  /* Media query for tablet and smaller screens */
  @media (max-width: 1024px) {
    .product-card {
      flex: 1 0 calc(50% - 1.25rem); /* Two products in a row with spacing */
      margin: 0 0.625rem;
      max-width: calc(50% - 1.25rem);
      padding: 0 0 2rem 0;
    }

    .description {
      height: 8.2rem;
    }
  }

  /* Media query for mobile screens */
  @media (max-width: 640px) {
    .product-card {
      max-width: 100%;
    }

    .description {
      height: 6rem;
    }

    p {
      font-size: 0.75rem;
    }
  }

  /* Media query for small mobile screens */
  @media (max-width: 280px) {
    .description {
      height: 8.2rem;
    }
  }
</style>
