<div class="hero-container">
  <img class="iris" src="../iris.jpeg" alt="iris flower" />
  <img class="hero" src="../hero.jpeg" alt="perfume bottles" />
</div>

<style>
  .hero-container {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: calc(100% - 0.025rem);
    overflow: hidden;
    gap: 0.2rem;
  }

  .iris {
    max-width: 30%;
    height: 100%;
    object-fit: cover;
  }

  .hero {
    max-width: 70%;
    height: 100%;
    object-fit: cover;
  }

  /* Media query for really large desktop screens */
  @media (max-width: 3840px) {
    .hero-container {
      height: 102rem;
    }
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .hero-container {
      height: 64rem;
    }
  }

  /* Media query for standard desktop screens */
  @media (max-width: 1920px) {
    .hero-container {
      height: 48rem;
    }
  }

  /* Media query for standard desktop screens */
  @media (max-width: 1440px) {
    .hero-container {
      height: 36rem;
    }
  }

  /* Media query for standard desktop screens */
  @media (max-width: 1280px) {
    .hero-container {
      height: 33rem;
    }
  }

  /* Media query for tablet and mobile screens */
  @media (max-width: 768px) {
    .hero-container {
      height: 30rem;
    }

    .iris {
      display: none;
    }

    .hero {
      max-width: 100%;
    }
  }
</style>
