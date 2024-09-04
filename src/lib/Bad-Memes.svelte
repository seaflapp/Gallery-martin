<script>
    // You can add props here if needed, e.g.:
    // export let images = [];
  
    const images = [
      { src: "/public/img/i-present-to-you-the-worlds-best-css-developer-v0-ug26me4gbb7d1.webp",  alt: "bilde av Nordlys" },
      { src: "/public/img/i-am-in-danger-v0-cm7870h02oad1.webp", alt: "bilde av Nordlys" },
      { src: "/public/img/new-programmers-v0-687x87ui5a6d1.webp",  alt: "bilde av Nordlys" },
    ];
  </script>
  
  <div class="Badmeme" id="Badmeme">
    <h2>Bad Memes</h2>
    <div class="image-container">
      {#each images as image}
        <img src={image.src} alt={image.alt} />
      {/each}
    </div>
  </div>


  <style>
    .Badmeme {
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