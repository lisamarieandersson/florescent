<script>
  import ContactForm from './ContactForm.svelte';
</script>

<div class="contact-container">
  <div class="line" />
  <div class="contact-headline"><h2>Contact us</h2></div>
  <div class="contact-content">
    <div class="customer-service-container">
      <h3>Help & FAQ</h3>
      <p>info@florescent-fragrances.com</p>
      <h3>Customer Service</h3>
      <p>Monday to Saturday</p>
      <p>10:00 AM to 06:00 PM (CEST)</p>
      <p>+46 411 419 35</p>
      <p>Live Chat</p>
    </div>
    <div class="press-wholesale-container">
      <h3>Press Inquiries</h3>
      <p>press@florescent-fragrances.com</p>
      <h3>Wholesale Inquiries</h3>
      <p>global_business@florescent-fragrances.com</p>
    </div>
    <div class="send-message">
      <h3>Send us a message</h3>
      <ContactForm />
    </div>
  </div>
</div>

<style>
  .contact-container {
    display: flex;
    flex-direction: column;
    margin-top: 2.5rem;
    padding: 0 50rem;
  }

  .contact-content {
    display: flex;
    flex-direction: row;
    gap: 6rem;
    padding: 0 34rem;
  }

  .contact-headline {
    text-align: center;
  }

  .send-message {
    flex: 2;
  }

  .line {
    height: 0.025rem;
    background: #000000;
  }

  h3 {
    font-weight: 400;
  }

  p {
    font-size: 0.875rem;
  }

  /* Media query for large desktop screens */
  @media (max-width: 2560px) {
    .contact-container {
      padding: 0 30rem;
    }

    .contact-content {
      padding: 0 15rem;
    }
  }

  /* Media queries for standard desktop screens */
  @media (max-width: 1920px) {
    .contact-container {
      padding: 0 2.125rem;
    }
  }

  /* Media query for standard desktop screens */
  @media (max-width: 1440px) {
    .contact-content {
      padding: 0;
    }

    .contact-headline {
      text-align: left;
    }
  }

  /* Media query for tablet screens */
  @media (max-width: 920px) {
    .contact-content {
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
    }
    h2 {
      margin-bottom: 1rem;
    }
  }

  /* Media query for mobile screens */
  @media (max-width: 640px) {
    .contact-container {
      padding: 0 1.5rem;
    }

    h2 {
      font-size: 1.8rem;
    }
  }
</style>
