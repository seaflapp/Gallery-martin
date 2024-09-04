<script>
    // You can add props here if needed, e.g.:
    // export let images = [];
  
    const images = [
      { src: "/public/img/true.jpeg",  alt: "java isn't stressful at all" },
      { src: "/public/img/not-my-code.jpg", alt: "bilde av Nordlys" },
      { src: "/public/img/iwanttostopcrying-v0-jqbyt6kneu9d1.webp",  alt: "bilde av Nordlys" },
    ];
  </script>
  
  <div class="Meme" id="Meme">
    <h2>Memes</h2>
    <div class="image-container">
      {#each images as image}
        <img src={image.src} alt={image.alt} />
      {/each}
    </div>
  </div>


  <style>
    .Meme {
      margin: 20px;
      padding: 20px;
      border: 1px solid #ddd;
      border-radius: 8px;
    }
  
    .image-container {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }
  
    img {
      max-width: 300px;
      height: auto;
      border-radius: 4px;
    }

    h2 {
      color: #242424;
    }
  </style>