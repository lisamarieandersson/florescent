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
  }

  img {
    max-width: 70%;
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
    width: 70%;
  }
</style>
