<script>
  export let selectedPage;
  export let naviPages;
</script>

<div class = "nav-section">
    <div class="navbar">
        <button class:selected={selectedPage === 'home'} 
       on:click={() => naviPages('home')}>Home</button>
        <button class:selected={selectedPage === 'resources'} 
        on:click={() => naviPages('resources')}>Resources</button>
        <button class:selected={selectedPage === 'mail'}
        on:click={() => naviPages('mail')}>Mail</button>
        </div>
</div>

<style>
  .nav-section {
    background-color: white;
    padding: 1rem 0;
    border-bottom: 1px solid #bb7091;
  }

  .navbar {
    display: flex;
    justify-content: center;
    gap: 2rem;
  }

  button {
    background: transparent;
    border: none;
    font-size: 1.1rem;
    color: #f487b6; 
    cursor: pointer;
    font-weight: 700;
  }

  button.selected {
    text-decoration: underline;
  }

  
</style>
