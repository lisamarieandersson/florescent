<script lang="ts">
  export let product: {
    name: string;
    image: string;
    description: string;
  };
</script>

<div class="product-card">
  <img src={product.image} alt={product.name} />
  <h3>{product.name}</h3>
  <p>{product.description}</p>
  <button>Add to Cart</button>
</div>

<style>
  .product-card {
    text-align: center;
    padding: 0 0.625rem;
    max-width: calc(25% - 0.025rem);
    box-sizing: border-box;
  }

  img {
    max-width: 100%;
    height: auto;
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

  /* Media query for tablet and larger screens */
  @media (max-width: 940px) {
    .product-card {
      flex: 1 0 calc(50% - 1.25rem); /* Two products in a row with spacing */
      margin: 0 0.625rem;
      max-width: calc(50% - 1.25rem);
    }
  }

  /* Media query for mobile screens */
  @media (max-width: 768px) {
    .product-card {
      max-width: 100%;
      padding: 0;
      margin-bottom: 2rem;
    }
  }
</style>
