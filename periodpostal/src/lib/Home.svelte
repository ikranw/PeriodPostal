<script>
  export let goDonate; 
  import homemadepads  from '../assets/homemadepads.jpg';
</script>

<section class="home">
  <h1 class="title">Period Postal</h1>

  <section class="home-section">
    <div class="home-text">
      <p>
        We are on a mission to promote access to menstrual products across the world.
        We aim to achieve this through donations, volunteer efforts, and community efforts of mailing handmade pads to 
        those who need them. Access to menstrual products shouldn't be limited to a zip code.<br />
        <br /> 1 in 4 teens and 1 in 3 adults struggle with access to menstrual products.<br />
       <br /> Make a difference and donate below.  <br />
      <br /> You can also check out the resource page to make handmade pads and mail them to those in need.  <br/>
    </p>
    </div>

    <div class="pad-img">
      <img src={homemadepads} alt="homemade pads" />
    </div>
  </section>

  <section class="donate-section">
    <button class="donate-button" on:click={goDonate}>
      DONATE
    </button>
  </section>
</section>

<style>
  .home {
    padding: 2rem 1.5rem 3rem;
  }

  .title {
    text-align: center;
    color: #e86da6;;
    margin-bottom: 2rem;
    font-size: 2.2rem;
  }

  .home-section {
    background-color: #ffe3f0; 
    border-radius: 10px;
    padding: 2rem;
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
    align-items: center;
    justify-content: space-between;
  }

  .home-text {
    flex: 1 1 250px;
    font-size: 1rem;
    line-height: 1.5;
    max-width: 500px;
  }

  .pad-img {
    flex: 1 1 200px;
    display: flex;
    justify-content: center;
  }

  .pad-img img {
    max-width: 260px;
    height: auto;
    border-radius: 8px;
  }

  .donate-section {
    background-color: #ffffff;
    padding: 2rem 0;
    display: flex;
    justify-content: center;
  }

  .donate-button {
    background-color: #ff4f9a;
    color: #ffffff;
    border: none;
    padding: 0.8rem 2.5rem;
    font-size: 1.1rem;
    font-weight: 600;
    border-radius: 999px;
    cursor: pointer;
    box-shadow: 0 4px 8px rgba(255, 79, 154, 0.35);
  }

  .donate-button:hover {
    transform: translateY(-1px);
  }
  
</style>
