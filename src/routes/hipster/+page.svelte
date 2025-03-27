<script>
  import { fade } from "svelte/transition"

  let y
  let height
  $: scrollPercentage = y / (1500 - height)
</script>

<svelte:window bind:scrollY={y} bind:innerHeight={height} />

<main>
  <section class="top">
    <h2>You Probably Haven't Heard of Hipster Ipsum</h2>

    <article>
      <article class="left-text">
        <p>Fingerstache tofu pickled vibecession kitsch lyft blackbird spyplane vegan craft beer keytar banh mi thundercats. Hashtag heirloom vape scenester paleo hexagon. Blackbird spyplane pok pok DIY heirloom scenester food truck kale chips pabst, bitters raw denim artisan waistcoat seitan freegan.</p>
      </article>
      <p>Put a bird on it vibecession fashion axe YOLO asymmetrical. VHS photo booth listicle fam truffaut subway tile yr cred chicharrones semiotics biodiesel green juice microdosing whatever. Truffaut praxis PBR and B tattooed street art. Prism jean shorts pickled vegan. Vegan praxis cronut kitsch pop-up. Letterpress street art mlkshk marxism.</p>
    </article>
  </section>

  <section class="middle">
    <h2>Build A Hipster Dude!</h2>
  </section>
  <section class="bottom">
    {#if scrollPercentage > 0.75}
      <img transition:fade class="hair" src="hipster-hairdo.png" alt="Hipster Hairdo" />
    {/if}
    {#if scrollPercentage > 0.9}
      <img transition:fade class="shirt" src="hipster-top.png" alt="Hipster Top" />
    {/if}
    {#if scrollPercentage > 1.05}
      <img transition:fade class="jeans" src="hipster-jeans.png" alt="Hipster Jeans" />
    {/if}
    {#if scrollPercentage > 1.15}
      <img transition:fade class="shoe-pair" src="Shoes-pair.png" alt="Hipster Shoes" />
    {/if}
  </section>
  <section class="extra"></section>
</main>

<style>
  h2 {
    font-family: "Monoton", sans-serif;
    transform: rotate(-10deg);
    padding: 5%;
    font-size: 450%;
    text-align: center;
  }

  .hair {
    height: 10%;
    width: 4%;
    transform: translateX(1198%);
    margin-top: 15.8%;
  }

  .shirt {
    height: 16%;
    width: 8%;
    transform: translateX(575%);
  }

  .jeans {
    height: 13.5%;
    width: 12%;
    transform: translateX(367%);
  }

  .shoe-pair {
    height: 3.6%;
    width: 6%;
    transform: translateX(785%);
  }

  p {
    font-family: "Marko One", serif;
    margin-left: 10%;
    margin-right: 5%;
    font-size: 120%;
  }
  .top {
    background-color: #f8e4c2;
    color: #7f353c;
    height: 700px;
  }

  .middle {
    background-color: #7f353c;
    color: #f8e4c2;
    height: 100px;
  }
  article {
    display: flex;
  }

  .left-text {
    margin-top: 40px;
  }

  .bottom {
    background-color: #7f353c;
    height: 700px;
    background-image: url("mannequin-for-hipster.png");
    background-repeat: no-repeat;
    background-position: center;
    display: flex;
    flex-direction: column;
  }

  .extra {
    background-color: #7f353c;
    height: 300px;
  }
</style>
