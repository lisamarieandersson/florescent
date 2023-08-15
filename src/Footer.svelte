<div class="footer-container">
  <div class="line" />
  <div class="footer-columns">
    <div class="info">
      <h3>Info</h3>
      <p>Shipping & Delivery</p>
      <p>Payment</p>
      <p>Returns & Refunds</p>
      <p>Terms of Use</p>
      <p>Privacy Policy</p>
      <p>Cookie Settings</p>
      <p>Accessibility Statement</p>
    </div>
    <div class="contact">
      <h3>Contact Us</h3>
      <p>Customer Care</p>
      <p>Live Chat</p>
      <p>FAQ</p>
      <p>Store Locator</p>
      <p>Stockists</p>
    </div>
    <div class="social">
      <h3>Social</h3>
      <p>Instagram</p>
      <p>Pinterest</p>
    </div>
    <div class="newsletter">
      <h3>Subscribe</h3>
      <div class="newsletter-form">
        <input type="email" placeholder="hello@example.com" />
        <button>Subscribe</button>
        <p>Enter your email address to receive special offers!</p>
      </div>
    </div>
  </div>
  <div class="symbol-and-logo">
    <img
      class="symbol"
      src="../symbol-florescent.svg"
      alt="symbol florescent"
    />
    <img
      class="logotype"
      src="../logotyp-florescent.svg"
      alt="logotype florescent"
    />
  </div>
  <div class="copy"><p>© 2023 Florescent</p></div>
</div>

<style>
  .footer-container {
    margin-top: 2.5rem;
    padding: 2.5rem 2.125rem 0.5rem 2.125rem;
    background-color: #f2efea;
  }

  .footer-columns {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr auto;
    /* max-width: 90rem; */
  }

  .line {
    height: 0.025rem;
    background: #000000;
    margin-bottom: 2.5rem;
  }

  .newsletter {
    display: flex;
    flex-direction: column;
  }

  h3 {
    text-transform: uppercase;
    margin-top: 0;
  }

  p {
    font-size: 0.875rem;
  }

  .newsletter p {
    margin-top: 0.5rem;
  }

  .newsletter-form input {
    padding: 0.5rem;
    border: solid 0.025rem #000000;
    border-radius: 0;
    margin-bottom: 0.5rem;
    padding: 0.9rem;
    font-family: 'Jost', sans-serif;
    font-weight: 300;
    width: 16rem;
  }

  .newsletter-form button {
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

  .newsletter-form button:hover {
    background: #ffffff;
    color: #000000;
  }

  .symbol-and-logo {
    display: flex;
    flex-direction: column;
    padding-bottom: 1rem;
  }

  .symbol {
    width: 6rem;
    height: auto;
    margin: 0 auto;
  }

  .logotype {
    padding-top: 0.8rem;
    width: 6rem;
    height: auto;
    margin: 0 auto;
  }

  .copy {
    text-align: center;
  }
  .copy p {
    font-size: 0.75rem;
  }

  /* Media query for mobile screens */
  @media (max-width: 820px) {
    .footer-columns {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      gap: 2rem;
    }

    .symbol-and-logo {
      padding-top: 2rem;
    }
  }
</style>
