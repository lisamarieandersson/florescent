<script>
  let name = '';
  let email = '';
  let phoneNumber = '';
  let message = '';

  function handleSubmit() {}
</script>

<div class="contact-form">
  <label for="name">Name</label>
  <input
    class="contact-input"
    type="text"
    id="name"
    placeholder="Name"
    bind:value={name}
  />
  <label for="email">Email</label>
  <input
    class="contact-input"
    type="email"
    id="email"
    placeholder="Email"
    bind:value={email}
  />
  <label for="phoneNumber">Phone Number</label>
  <input
    class="contact-input"
    type="tel"
    id="phoneNumber"
    placeholder="Phone Number"
    bind:value={phoneNumber}
  />
  <label for="message">Message</label>
  <textarea
    class="contact-message"
    id="message"
    rows="5"
    placeholder="Write your message here"
    bind:value={message}
  />
  <button class="contact-button" on:click={handleSubmit}>Submit</button>
</div>

<style>
  .contact-form {
    display: flex;
    flex-direction: column;
  }

  .contact-input {
    padding: 0.5rem;
    border: solid 0.025rem #000000;
    border-radius: 0;
    margin-bottom: 0.5rem;
    padding: 0.9rem;
    font-family: 'Jost', sans-serif;
    font-weight: 300;
  }

  .contact-message {
    border: solid 0.025rem #000000;
    margin-bottom: 0.625rem;
    padding: 0.9rem;
    font-family: 'Jost', sans-serif;
    font-weight: 300;
  }

  .contact-button {
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

  .contact-button:hover {
    background: #ffffff;
    color: #000000;
  }

  label {
    font-family: 'Jost', sans-serif;
    font-weight: 300;
    font-size: 0.875rem;
    padding-bottom: 0.5rem;
  }
</style>
