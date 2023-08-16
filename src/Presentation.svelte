<div class="presentation-container">
  <div class="presentation-text">
    <h1>Fragrances for your everyday life.</h1>
    <p class="padding-bottom">
      Florescent is a lifestyle fragrance brand created for, and inspired by
      your most honest self. Based on the finest raw materials and delicate
      perfumery, we present a fragrance line that creates a mysterious and
      unique mood. You'll find that most of our scents are inspired by our love
      for florals, but in our fragrance collection you'll also find fragrances
      with more woody and earthy tones. All waiting to be a part of your scented
      wardrobe.
    </p>
    <button>Read more</button>
  </div>
</div>

<style>
  .presentation-container {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 100%;
    overflow: hidden;
    background-color: #f2efea;
    padding: 4rem 0;
    margin-top: 4rem;
  }

  .presentation-text {
    max-width: 20%;
    text-align: center;
  }

  .padding-bottom {
    padding-bottom: 1rem;
  }

  .presentation-text button {
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

  h1 {
    margin-top: 0;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .presentation-text {
      max-width: 30%;
    }
  }

  /* Media query for standard desktop screens */
  @media (max-width: 1440px) {
    .presentation-text {
      max-width: 45%;
    }
  }

  /* Media query for smaller desktop and tablet screens */
  @media (max-width: 1024px) {
    .presentation-container {
      margin-top: 2rem;
    }
  }

  /* Media query for tablet and mobile screens */
  @media (max-width: 768px) {
    .presentation-text {
      max-width: 80%;
    }
  }
</style>
