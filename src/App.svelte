<script>
  import Header from './lib/Header.svelte'
  import Footer from './lib/Footer.svelte';
  import Gallery from './lib/Gallery.svelte';
  import Gallery2 from './lib/Gallery2.svelte';
  import Hero from './lib/Hero.svelte';
  import Intro from './lib/Intro.svelte';
  
  let showGallery = false;

  function toggleGallery() {
    showGallery = !showGallery;
  }
</script>



<main>
  <Header />
  <Hero />
  <Intro />
  
  <button on:click={toggleGallery}>
    {showGallery ? 'Remove Gallery' : 'Show Gallery'}
  </button>
  {#if showGallery}
    <Gallery />
  {/if}
  {#if showGallery}
    <Gallery2 />
  {/if}
  <Footer />
</main>


<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }

  button {
    font-size: 1em;
    padding: 10px 20px;
    margin: 20px 0;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

  button:hover {
    background-color: #45a049;
  }
</style>