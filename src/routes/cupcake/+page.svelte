<script>
  let y
  let height
  $: scrollPercentage = y / (6000 - height)
</script>

<svelte:window bind:scrollY={y} bind:innerHeight={height} />

<main>
  <h2>Cupcake Ipsum</h2>

  <div class="cupcake_layout_div">
    <div class="text">
      <p>Halvah liquorice apple pie jelly beans chupa chups candy icing tiramisu. Tart jelly jujubes gingerbread croissant biscuit. Chupa chups tart cheesecake lemon drops dragée chocolate bar dessert. Ice cream ice cream sugar plum jujubes dragée topping tiramisu croissant chocolate.</p>
      <p>Jujubes tiramisu gingerbread cake donut chocolate bar tart marzipan pastry. Gingerbread jelly tootsie roll muffin bear claw muffin. Jelly-o fruitcake chocolate bar chupa chups chocolate sesame snaps candy. Sweet roll carrot cake cake jelly candy jujubes gummi bears jelly-o. Oat cake wafer chocolate bar sweet roll macaroon soufflé powder sugar plum tart.</p>
    </div>
    {#if scrollPercentage >= 0.37}
      <div class="explosion" style="top: 10vh;"></div>
      <img src="splatter-4.webp" alt="Splatter" style="top:2vh; height:70vh;" />
      <img src="splatter-4.webp" alt="Splatter" style="left:2vh; height:80vh;" />
      <img src="splatter-4.webp" alt="Splatter" style="bottom:2vh; height:65vh;" />
    {/if}
    {#if scrollPercentage < 0.37}
      <img src="Cupcake-notlit-sparkler.png" alt="Cupcake with sparkler on top" style="left:15vh;" />
      <img src="sparkle.png" alt="Sparkler light" style="top: {45 + scrollPercentage * 40}vh; left: {scrollPercentage * 60}vh;" />
    {/if}
  </div>
</main>

<style>
  h2 {
    font-family: "Ingrid Darling", system-ui;
    font-size: 1800%;
    text-align: center;
    color: #ffdff4;
  }

  p {
    color: #ffdff4;
    margin-right: 200px;
    margin-left: 700px;
    font-size: 325%;
    font-family: "Lily Script One", system-ui;
  }

  img {
    position: fixed;
    margin-left: 40px;
    height: 200px;
  }

  .explosion {
    position: fixed;
    margin-left: 40px;
    height: 800px;
    width: 800px;
    background-image: url("giphy-explosion.gif");
    background-repeat: no-repeat;
  }

  main {
    background-color: #8b3683;
    height: 5000px;
  }

  .text {
    display: column;
  }

  .cupcake_layout_div {
    display: flex;
  }

  /*Need to make div not appear until it hits a certain scroll percentage and at that point, hide the cupcake and sparkler.
  div code previously used*/
</style>
