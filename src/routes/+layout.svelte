<slot />

<style>
  @import url("https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Irish+Grover&family=Manrope:wght@200..800&family=Nunito:ital,wght@0,200..1000;1,200..1000&family=Salsa&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Ingrid+Darling&family=Lily+Script+One&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Marko+One&family=Monoton&display=swap");

  /* The code below resets the browser's default styles. It's a good idea to include this in your layout component. */
  :global(body) {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
  }

  :global(a) {
    color: #1eaedb;
    text-decoration: none;
  }

  :global(a:hover) {
    color: #0fa0ce;
  }

  :global(h1) {
    font-size: 2rem;
    font-weight: 300;
    margin: 0 0 1rem 0;
  }

  :global(h2) {
    font-size: 1.5rem;
    font-weight: 300;
    margin: 0 0 1rem 0;
  }

  @font-face {
    font-family: hyper-scrypt;
    src: url("/HyperScrypt-Stencil_web.woff2") format("woff2");
  }

  @font-face {
    font-family: basteleur;
    src: url("/Basteleur-Moonlight.woff2") format("woff2");
  }
</style>
