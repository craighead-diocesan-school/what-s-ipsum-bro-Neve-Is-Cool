<script>
  let y
  let height
  $: scrollPercentage = y / (1500 - height)
</script>

<svelte:window bind:scrollY={y} bind:innerHeight={height} />

<main>
  <div class="cheese">
    <img class="is-rounded" src="c-for-cheese.png" alt="Cheese heading with round cheese for the C" />
    <h2>heese Ipsum</h2>
  </div>

  <div class="text-background">
    <p>Cheesy grin parmesan taleggio. Brie boursin pecorino cheesy feet taleggio hard cheese roquefort when the cheese comes out everybody's happy. St. agur blue cheese port-salut bocconcini cheesecake rubber cheese mozzarella stilton cheese strings. Bocconcini.</p>

    <p>Fromage the big cheese camembert de normandie. Cut the cheese gouda brie the big cheese when the cheese comes out everybody's happy squirty cheese cut the cheese gouda. Boursin cottage cheese cheeseburger camembert de normandie cheese slices goat port-salut danish fontina. Emmental caerphilly cream cheese mozzarella camembert de normandie cheesy feet.</p>
  </div>
</main>

<style>
  main {
    background-color: #dc4d3a;
  }

  img {
    height: 150px;
    width: 150px;
    border-radius: 50%;
    margin-left: 5%;
  }

  p {
    font-family: "Irish Grover", system-ui;
    color: #f7d571;
    margin-left: 20%;
    margin-right: 30%;
    transform: rotate(-10deg);
    transition: 0.5s;
  }

  p:hover {
    color: #f2b329;
    scale: 1.1;
    transform: rotate(0deg);
    background-color: #dc4d3a;
    transition: 0.5s;
  }

  .text-background {
    background-image: url("Gouda-block-slice.png");
    background-repeat: no-repeat;
    background-position: center;
    padding-bottom: 200px;
    padding-left: 200px;
    padding-right: 200px;
    padding-top: 100px;
  }
  h2 {
    color: #f2b329;
    font-family: "Irish Grover", system-ui;
    font-size: 1000%;
  }

  .cheese {
    display: flex;
    align-items: center;
  }
</style>
