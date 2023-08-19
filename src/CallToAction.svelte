<div class="call-to-action-container">
  <img class="orchids" src="../orchids.jpeg" alt="orchid flowers" />
  <img class="perfume-bottle" src="perfume-bottle.png" alt="perfume bottle" />
  <div class="text-container">
    <h2>Discover our collection</h2>
    <p class="padding-bottom">
      Our fragrances are crafted with high-quality ingredients that are sourced
      by top-tier perfumers of global renown, giving each product a unique
      narrative. We never compromise on product and scent development. Each
      ingredient is curated and sourced by carefully selected partners around
      the world, allowing us to offer products of purest quality and exceptional
      experiences.
    </p>
    <button>Shop now</button>
  </div>
</div>

<style>
  .call-to-action-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    max-width: 100%;
    background-color: #f2efea;
    padding: 4rem 50rem 4rem 50rem;
    gap: 1.25rem;
    margin-top: 4rem;
  }

  .orchids,
  .perfume-bottle {
    flex: 1;
    max-width: 33%;
    height: auto;
  }

  .text-container {
    text-align: center;
    max-width: 33%;
  }

  h2 {
    font-weight: 400;
    font-size: 2.3rem;
    margin-top: 0;
    margin-bottom: 1rem;
  }

  .perfume-bottle {
    padding-top: 5rem;
  }

  .padding-bottom {
    padding-bottom: 1rem;
  }

  button {
    border-radius: 0;
    font-family: 'Fraunces', serif;
    font-weight: 300;
    background: #000000;
    color: #ffffff;
    border: solid 0.025rem #000000;
    padding: 1rem;
    text-transform: uppercase;
    text-align: center;
    cursor: pointer;
  }

  button:hover {
    background: #ffffff;
    color: #000000;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .call-to-action-container {
      padding: 4rem 30rem 4rem 30rem;
    }
  }
  /* Media queries for standard desktop screens */
  @media (max-width: 1920px) {
    .call-to-action-container {
      padding: 4rem 2.125rem 4rem 2.125rem;
    }
  }

  /* Media query for tablet and mobile screens */
  @media (max-width: 768px) {
    .call-to-action-container {
      flex-direction: column-reverse;
      justify-content: center;
      align-items: center;
      gap: 1.25rem;
    }

    .orchids,
    .perfume-bottle {
      max-width: 100%;
      height: auto;
    }

    .perfume-bottle {
      padding-top: 0;
    }

    .text-container {
      text-align: center;
      max-width: 100%;
    }
  }

  @media (max-width: 640px) {
    .call-to-action-container {
      padding: 4rem 1.5rem 4rem 1.5rem;
    }
  }
</style>
