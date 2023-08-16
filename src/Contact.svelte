<script>
  import ContactForm from './ContactForm.svelte';
</script>

<div class="contact-container">
  <div class="contact-header"><h2>Contact us</h2></div>
  <div class="contact-content">
    <div class="customer-service-container">
      <h3 class="margin-bottom">Help & FAQ</h3>
      <div class="line" />
      <p class="padding-bottom">info@florescent-fragrances.com</p>
      <h3 class="margin-bottom">Customer Service</h3>
      <div class="line" />
      <p>Monday to Saturday</p>
      <p>10:00 AM to 06:00 PM (CEST)</p>
      <p>+46 411 419 35</p>
      <p>Live Chat</p>
    </div>
    <div class="press-wholesale-container">
      <h3 class="margin-bottom">Press Inquiries</h3>
      <div class="line" />
      <p class="padding-bottom">press@florescent-fragrances.com</p>
      <h3 class="margin-bottom">Wholesale Inquiries</h3>
      <div class="line" />
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
    padding: 0 50rem;
  }

  .contact-content {
    display: flex;
    flex-direction: row;
    gap: 6rem;
    padding: 0 34rem;
  }

  .contact-header {
    text-align: center;
    height: 5rem;
  }

  .send-message {
    flex: 2;
  }

  .line {
    height: 0.025rem;
    background: #000000;
  }

  .padding-bottom {
    padding-bottom: 1rem;
  }

  .margin-bottom {
    margin-bottom: 0.4rem;
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

    .contact-header {
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
  }

  /* Media query for mobile screens */
  @media (max-width: 640px) {
    .contact-container {
      padding: 0 1.5rem;
    }
  }
</style>
