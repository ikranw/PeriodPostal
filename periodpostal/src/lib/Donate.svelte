<script>
  export let submitButton = () => {};
  export let cancelButton = () => {};

  function handleSubmit() {
     alert("You have successfully donated! Thank you for your support.");
    submitButton?.();
  }
</script>

<div class="donate-page">
  <div class="heading">Donation for Period Postal</div>

  <div class="donate-content">
    <div class="amount-field">
      <label for="amount">Amount (USD):</label>
      <input id="amount" type="number" step="0.01" min="0" placeholder="0.00" />
    </div>

    <div class="occur-field">
      <label for="occurrences">Occurrences:</label>
      <select id="occurrences">
        <option value="one-time">One-time donation</option>
        <option value="weekly">Weekly donations</option>
        <option value="monthly">Monthly donations</option>
        <option value="yearly">Yearly donations</option>
      </select>
    </div>

    <div class="card-section">
      <div class="card-heading">Card Information</div>

      <div class="cardfield-row">
        <div class="field">
          <label for="first-name">First Name:</label>
          <input id="first-name" type="text" />
        </div>

        <div class="cardfield">
          <label for="last-name">Last Name:</label>
          <input id="last-name" type="text" />
        </div>
      </div>

      <div class="cardfield">
        <label for="card-number">Card Number:</label>
        <input id="card-number" type="text" placeholder="0000-0000-0000-0000" />
      </div>

      <div class="cardfield-row">
        <div class="cardfield">
          <label for="security-code">Security Code:</label>
          <input id="security-code" type="text" placeholder="123" />
        </div>

        <div class="cardfield">
          <label for="exp">Expiration Date:</label>
          <input id="exp" type="text" placeholder="YYYY/MM" />
        </div>
      </div>
    </div>

    <div class="email-field">
      <label for="email">Email:</label>
      <input id="email" type="text" placeholder="you@gmail.com" />
    </div>

    <div class="actions">
      <button type="button" class="submit" on:click={handleSubmit}>
        Submit
      </button>
      <button type="button" class="cancel" on:click={() => { 
        alert("Donation was canceled."); cancelButton();}}>
        Cancel
      </button>
    </div>
  </div>
</div>

<style>
  .donate-page {
    max-width: 550px;
    margin: 1.5rem auto;
    padding: 2rem;
    background-color: #ffffff;
    border-radius: 12px;
    box-shadow: 0 10px 16px rgba(188, 10, 10, 0.08);
  }

  .heading {
    text-align: center;
    font-size: 1.4rem;
    font-weight: 500;
    margin-bottom: 1.8rem;
    color: #f693c1;
  }

  .donate-content {
    display: flex;
    flex-direction: column;
    gap: 1.1rem;
  }

  .cardfield {
    display: flex;
    flex-direction: column;
    gap: 0.3rem;
  }
  .amount-field, .occur-field, .email-field {
    display: flex;
    flex-direction: column;
    gap: 0.3rem;
    color: #f693c1;
  }
  .cardfield-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.75rem;
  }

  label {
    font-size: 1rem;
    font-weight: 600;
    color: #f693c1
  }
   .card-section label{
    font-size: 1rem;
    font-weight: 200;
    color: #050505
  }

  input,
  select {
    padding: 0.65rem 0.75rem;
    border-radius: 6px;
    border: 1px solid #dddddd;
    font-size: 1rem;
  }

  .card-section {
    padding: 1rem;
    border-radius: 10px;
    background-color: #ffe3f0;
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .card-heading {
    font-weight: 700;
    margin-bottom: 0.25rem;
    color: #000000;
  }

  .actions {
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    gap: 0.75rem;
    margin-top: 1.5rem;
  }

  .submit {
    background-color: #ff4f9a;
    color: #ffffff;
    border: none;
    padding: 0.6rem 1.4rem;
    border-radius: 999px;
    font-weight: 600;
    cursor: pointer;
  }

  .cancel {
    background-color: #ffffff;
    color: #ff0000;
    border: 1px solid #ff0000;
    padding: 0.6rem 1.4rem;
    border-radius: 999px;
    font-weight: 600;
    cursor: pointer;
  }
</style>
