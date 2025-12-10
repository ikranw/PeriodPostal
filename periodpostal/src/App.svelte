<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Home from './lib/Home.svelte';
  import Donate from './lib/Donate.svelte';
  import Resources from './lib/Resources.svelte';
  import Mail from './lib/Mail.svelte';
  import Nav from './lib/Nav.svelte';

  let selectedPage = 'home';

  function naviPages(page) {
    selectedPage = page;
  }

  function goDonate() {
    selectedPage = 'donate';
  }

  function goHome() {
    selectedPage = 'home';
  }
</script>

<main>
  <Nav {selectedPage} {naviPages} />

  {#if selectedPage === 'home'}
    <Home {goDonate} />
  {:else if selectedPage === 'resources'}
    <Resources />
  {:else if selectedPage === 'mail'}
    <Mail />
  {:else if selectedPage === 'donate'}
    <Donate submitButton={goHome} cancelButton={goHome} />
  {/if}
</main>

<style>
  main {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    min-height: 100vh;
    background-color: white;
  }
</style>
