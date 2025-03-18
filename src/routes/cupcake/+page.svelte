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
    <img src="Cupcake-notlit-sparkler.png" alt="Cupcake with sparkler on top" style="left:15vh;" />
    <img src="sparkle.png" alt="Sparkler light" style="top: {45 + scrollPercentage * 20}vh; left: {scrollPercentage * 30}vh;" />
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
    margin-right: 50px;
    margin-left: 600px;
    font-size: 325%;
    font-family: "Lily Script One", system-ui;
  }

  img {
    position: fixed;
    margin-left: 40px;
    height: 200px;
  }

  main {
    background-color: #8b3683;
    height: 10000px;
  }

  .text {
    display: column;
  }

  .cupcake_layout_div {
    display: flex;
  }
</style>
