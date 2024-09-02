<script>
    // You can add props here if needed, e.g.:
    // export let images = [];
  
    const images = [
      { src: "/public/img/nordlys14.jpg", alt: "bilde av Nordlys" },
      { src: "/public/img/nordlys12.jpg", alt: "bilde av Nordlys" },
      { src: "/public/img/nordlys11.jpg", alt: "bilde av Nordlys" },
    ];
  </script>
  
  <div class="gallery" id="Gallery">
    <h2>Image Gallery2</h2>
    <div class="image-container">
      {#each images as image}
        <img src={image.src} alt={image.alt} />
      {/each}
    </div>
  </div>
  
  <style>
    .gallery {
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
  </style>