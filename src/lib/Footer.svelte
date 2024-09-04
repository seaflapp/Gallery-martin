<footer id="contacts">
    <div class="contact-info">
      <p>Telefon:</p>
      <p>Adresse:</p>
      <p>
        Email:
        <a href="mailto:martin.digitaletalenter@gmail.com"
          >martin.digitaletalenter@gmail.com</a
        >
      </p>
    </div>

    <nav>
      <a href="#intro">intro</a>
      <a href="#Gallery">Gallery</a>
      <a href="#Top-of-page">Top of page </a>
    </nav>
  </footer>

<style>
footer {
    display: flex;
    background-color: var(--tertiery);
    height: 96px;
    padding-inline: 32px;
    justify-content: space-between;
    align-items: center;
}

footer div.contact-info {
    /* display: grid; */
    /* background-color: rgb(26, 26, 20); */
    /* gap: 2px; */
   text-align: left;
}

footer div.contact-info a {
    color: var(--link);
}

footer nav {
    display: flex;
    flex-direction: column;
    gap: 8px;
}

footer nav a {
    color: var(--link);
}

footer nav a:hover {
    scale: 120%;
}

footer nav a:active {
    scale: 90%;
}
</style>