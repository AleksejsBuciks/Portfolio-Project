<script>

</script>

<section class="contact-form">
    <h2>Got Questions?</h2>
    <form on:submit|preventDefault>
      <label for="name">NAME</label>
      <input id="name" type="text" placeholder="Your Name" />
  
      <label for="email">Email Address</label>
      <input id="email" type="email" placeholder="your@email.com" />
  
      <label for="message">Message</label>
      <textarea id="message" rows="5">Example Text</textarea>
  
      <button type="submit">Send</button>
    </form>
  </section>

<style>

.contact-form {
    background-color: #243447;
    padding: 40px;
    color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 100px;
  }

  .contact-form h2 {
    color: #a100f2;
    font-size: 2rem;
    margin-bottom: 2rem;
  }

  .contact-form form {
    display: flex;
    flex-direction: column;
    width: 300px;
  }

  .contact-form label {
    margin-bottom: 5px;
    font-weight: bold;
    font-size: 0.85rem;
  }

  .contact-form input,
  .contact-form textarea {
    background-color: #121e2a;
    border: none;
    padding: 10px;
    margin-bottom: 15px;
    border-radius: 8px;
    color: white;
  }

  .contact-form textarea {
    resize: none;
  }

  .contact-form button {
    background-color: #a100f2;
    border: none;
    padding: 10px;
    border-radius: 25px;
    color: white;
    font-size: 1rem;
    cursor: pointer;
    transition: background-color 0.3s;
  }

  .contact-form button:hover {
    background-color: #8000c2;
  }

</style>