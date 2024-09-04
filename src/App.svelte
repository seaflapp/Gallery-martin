<script>
  import Header from './lib/Header.svelte'
  import Footer from './lib/Footer.svelte';
  import Gallery from './lib/Gallery.svelte';
  import Gallery2 from './lib/Gallery2.svelte';
  import Hero from './lib/Hero.svelte';
  import Intro from './lib/Intro.svelte';
  import Memes from './lib/Memes.svelte';
  import BadMemes from './lib/Bad-Memes.svelte';
  import Trolls from './lib/Trolls.svelte';
  
  let showGallery = false;
  let showMeme = false;
  let showBadmeme =false;
  let showTroll =false;

function toggleGallery() {
  showGallery = !showGallery;
}
function togglememe() {
  showMeme = !showMeme;
}
function togglebadmemes() {
  showBadmeme = !showBadmeme;
}
function toggletroll() {
  showTroll = !showTroll;
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
  <h3> test of multiple galleries</h3>
  <button on:click={togglememe}>
    {showMeme ? 'Remove Memes' : 'Memes'}
  </button>  <button on:click={togglebadmemes}>
    {showBadmeme ? 'Remove Bad Memes' : 'Bad Memes'}
  </button>  <button on:click={toggletroll}>
      <a href="https://emoji.gg/emoji/3846-troll"><img src="https://cdn3.emoji.gg/emojis/3846-troll.gif" width="64px" height="64px" alt="troll"></a>
  </button>
  {#if showMeme}
    <Memes />
  {/if}
  {#if showBadmeme}
    <BadMemes />
  {/if}
  {#if showTroll}
    <Trolls />
  {/if}

  <Footer />
</main>


<style>
  main {
    text-align: center;
    /* padding: 1em; */
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
  a {
    mix-blend-mode: multiply;
  }
</style>