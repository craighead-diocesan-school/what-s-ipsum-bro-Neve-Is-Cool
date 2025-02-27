<main>
  <div class="subheader">
    <img src="poison.png" alt="pirate skull" />
    <h2>Yar Pirate Ipsum</h2>
    <img src="poison.png" alt="pirate skull" />
  </div>
  <div class="waves">
    <div class="shipbackground">
      <div class="background">
        <p>Maroon square-rigged rope's end spirits fathom tackle bilge rat careen cackle fruit splice the main brace. Arr to go on account bilge six pounders smartly yo-ho-ho yawl tack boatswain maroon. Barque hogshead coffer Buccaneer loot fire ship Shiver me timbers Blimey salmagundi reef.</p>
      </div>
      <div class="background">
        <p>Draft scuttle rigging shrouds blow the man down belaying pin cog fluke strike colors killick. Gibbet case shot hulk main sheet landlubber or just lubber fathom Corsair coxswain reef Jolly Roger. Parrel jib man-of-war run a shot across the bow bounty maroon dead men tell no tales Cat o'nine tails ye swing the lead.</p>
      </div>
    </div>
  </div>
</main>

<style>
  .subheader {
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-image: url("Black-Flag.png");
    padding-top: 50px;
    padding-bottom: 50px;
  }

  .background {
    background-color: rgba(255, 255, 255, 0.5);
    padding: 10px;
    margin-left: 150px;
    margin-right: 150px;
    margin-bottom: 40px;
    transition: 0.25s;
  }

  .background:hover {
    background-color: white;
    transition: 0.25s;
  }

  .shipbackground {
    background-image: url("ship.gif");
    background-position: bottom;
    background-repeat: no-repeat;
    padding-bottom: 11%;
  }
  .waves {
    background-image: url("waves.gif");
    background-position: bottom;
    padding-top: 4%;
  }

  h2 {
    font-family: "hyper-scrypt";
    color: #d9edff;
    font-size: 375%;
    transition: 1s;
  }

  p {
    font-family: basteleur;
  }

  h2:hover {
    color: #880808;
    transition: 1.5s;
  }

  img {
    width: 6%;
    height: 6%;
  }
</style>
