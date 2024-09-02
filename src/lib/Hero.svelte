 <section class="hero">
     <div class="hero-text">
       <h1>Min samling av nordlysbilder</h1>
       <!-- <p>Jeg liker å ta bilder når det er nordlys ute</p> -->
      </div>
      <button>
         <a href="#Gallery">Gallery</a>
      </button>
  </section>





<style>
section.hero {
    min-height: calc(105dvh - 80px);
    background-color: transparent;
    border: none;
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
    gap: 32px;
    /* background-color: var(--quertiery); */
    border-radius: 0;
    margin-inline: 0;
    margin-top: 0;
    background-image: url(/public/img/nordlys12.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

section.hero div.hero-text {
    display: grid;
    gap: 0px;
}

section.hero h1 {
    font-size: 2.5rem;
    color: #aabfd3;
}

section.hero button {
    background-color: rgba(143, 143, 143, 0.123);
    border: 2px solid rgba(59, 58, 58, 0.281);
    border-radius: 8px;
    padding: 4px;
    box-shadow: 2px 2px 3px #252525;
}
</style>