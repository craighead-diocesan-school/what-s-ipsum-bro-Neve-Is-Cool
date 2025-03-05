<script>
  let y
  let height
  $: scrollPercentage = y / (1500 - height)
</script>

<svelte:window bind:scrollY={y} bind:innerHeight={height} />

<main>
  <img class="is-rounded" src="c-for-cheese.png" alt="Cheese heading with round cheese for the C" />

  <h2>heese Ipsum</h2>

  <div class="text-background">
    <p>Cheesy grin parmesan taleggio. Brie boursin pecorino cheesy feet taleggio hard cheese roquefort when the cheese comes out everybody's happy. St. agur blue cheese port-salut bocconcini cheesecake rubber cheese mozzarella stilton cheese strings. Bocconcini.</p>

    <p>Fromage the big cheese camembert de normandie. Cut the cheese gouda brie the big cheese when the cheese comes out everybody's happy squirty cheese cut the cheese gouda. Boursin cottage cheese cheeseburger camembert de normandie cheese slices goat port-salut danish fontina. Emmental caerphilly cream cheese mozzarella camembert de normandie cheesy feet.</p>
  </div>

  <aside style="transform: rotate({scrollPercentage * 1000}deg);"></aside>
</main>

<!--I might need these so I'm not deleting them yet.-->
<!----------transform: translateX(30%);-------------->
<!----------transform: rotate({scrollPercentage * 1000}deg);-------------->

<style>
  main {
    height: 2500px;
    background-color: #dc4d3a;
  }

  img {
    height: 150px;
    width: 150px;
    border-radius: 50%;
  }

  p {
    font-family: "Irish Grover", system-ui;
    color: #f7d571;
    margin-left: 20%;
    margin-right: 30%;
    transform: rotate(-10deg);
  }

  .text-background {
    background-image: url("Gouda-block-slice.png");
    background-repeat: no-repeat;
    background-position: center;
    padding: 200px;
  }
  h2 {
    color: #f2b329;
    font-family: "Irish Grover", system-ui;
    font-size: 1000%;
    text-align: center;
  }

  aside {
    position: fixed;
    width: 100px;
    height: 100px;
    background-image: url("Cheese-squares.jpg");
    transform: translateX(100%);
    transform: translateY(100%);
  }
</style>
