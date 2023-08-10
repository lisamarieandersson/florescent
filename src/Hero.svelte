<div class="hero-container">
  <img class="iris" src="../iris.jpeg" alt="iris flower" />
  <img class="hero" src="../hero.jpeg" alt="perfume bottles" />
</div>

<style>
  .hero-container {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 100%;
    overflow: hidden;
  }

  .iris {
    max-width: 30%;
    height: auto;
  }

  .hero {
    max-width: 71.1%;
    height: auto;
  }

  /* Media query for mobile screens */
  @media (max-width: 768px) {
    .iris {
      display: none;
    }

    .hero {
      max-width: 100%;
    }
  }
</style>
