<div class="footer-container">
  <div class="line" />
  <div class="footer-columns">
    <div class="newsletter">
      <h3>Subscribe</h3>
      <div class="newsletter-form">
        <input type="email" placeholder="hello@example.com" />
        <button>Subscribe</button>
        <p>Enter your email address to receive special offers!</p>
      </div>
    </div>
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
  </div>
  <div class="symbol-logo">
    <img src="../symbol-florescent.svg" alt="symbol florescent" />
  </div>
  <div class="copy"><p>© 2023 Florescent</p></div>
</div>

<style>
  .footer-container {
    margin-top: 2.5rem;
    padding: 2.5rem 1.5rem;
    background-color: #f2efea;
  }

  .footer-columns {
    display: grid;
    grid-template-columns: auto 1fr 1fr 1fr;
    gap: 3rem;
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

  .symbol-logo {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 6rem;
    height: auto;
    margin: 0 auto;
  }

  .info {
    display: flex;
    flex-direction: column;
  }

  .info p {
    margin: 0.3rem;
  }

  .copy {
    text-align: center;
  }
</style>
