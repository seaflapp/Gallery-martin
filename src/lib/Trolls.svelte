<script>
    // You can add props here if needed, e.g.:
    // export let images = [];
  
    const images = [
      { src: "/public/img/progmeme.jpeg",  alt: "bilde av Nordlys" },
      { src: "/public/img/s2jycx2kwa6d1.webp", alt: "bilde av Nordlys" },
      { src: "/public/img/i-think-so-v0-bojkcdtbk76d1.webp",  alt: "bilde av Nordlys" },
    ];
  </script>
  
  <div class="Troll" id="Troll">
    <h2>Never gonna give you up <a href="https://emoji.gg/emoji/1053-getrickrolled"><img src="https://cdn3.emoji.gg/emojis/1053-getrickrolled.gif" width="128px" height="128px" alt="GetRickRolled"></a> </h2>
    <div class="image-container">
      {#each images as image}
        <img src={image.src} alt={image.alt} />
      {/each}
    </div>
  </div>


  <style>
    .Troll {
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