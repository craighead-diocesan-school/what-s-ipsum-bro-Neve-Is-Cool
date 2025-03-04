<script>
  let y
  let height
  $: scrollPercentage = y / (1500 - height)
</script>

<svelte:window bind:scrollY={y} bind:innerHeight={height} />

<main>
  <h2>Pee-YOO Cheese Ipsum</h2>

  <p>Cheesy grin parmesan taleggio. Brie boursin pecorino cheesy feet taleggio hard cheese roquefort when the cheese comes out everybody's happy. St. agur blue cheese port-salut bocconcini cheesecake rubber cheese mozzarella stilton cheese strings. Bocconcini.</p>

  <p>Fromage the big cheese camembert de normandie. Cut the cheese gouda brie the big cheese when the cheese comes out everybody's happy squirty cheese cut the cheese gouda. Boursin cottage cheese cheeseburger camembert de normandie cheese slices goat port-salut danish fontina. Emmental caerphilly cream cheese mozzarella camembert de normandie cheesy feet.</p>

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

  h2 {
    color: #f2b329;
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
