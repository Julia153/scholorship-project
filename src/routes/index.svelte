<style>
/*making the title be centered */
  .title {
    text-align: center;
  }

/* changing the buttons to look how I want them from the bulma default button class*/
  .button {
    width: 300px;
    height: 300px;
    margin: 20px;
    border-style: solid;
    border-width: 10px;
    border-color: #1d3461;
    border-radius: 10px;
    background-color: #f5f6f4;
  }

/* Making all of the buttons centered on the screen*/
  #container1-3 {
    height: 200px;
    position: relative;
  }

  #vertical-center1-3 {
    margin: 0;
    position: absolute;
    right: 10%;
    top: 80%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #container3-5 {
    height: 200px;
    position: relative;
  }

  #vertical-center3-5 {
    margin: 0;
    position: absolute;
    right: 24%;
    top: 150%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

/* Setting the background color, and height of the page*/
  #body {
    background-color: #80cddb;
    height: 1000px;
    margin: 0px;
  }

/* Changing the color of the buttons for settings and to log out*/
  #logOutLink,
  #settingsLink {
    color: #1d3461;
    font-size: 30px;
    text-decoration: underline;
    text-decoration-line: underline;
    margin: 10px;
  }
</style>

<!--Div for whole page to set background color-->
<div id="body">
<!--Setting my title to be my SkyShip logo-->
  <h1 class="title">
    <img
      style="height: 20%; width: auto; "
      src="SkyShipTitle.png"
      alt="SkyShip title words sky ship in clouds with a rocket launching" />
  </h1>
<!--Button to logout-->
  <a id="logOutLink" href="/login">Log Out</a>
  <!--Button to go to settings-->
  <a id="settingsLink" href="/settings">Settings</a>

  <!--Buttons for emotions-->
  <div id="container1-3">
    <div id="vertical-center1-3">
      <a id="emotions" href="/emotions">
        <button class="button">
        <i style="font-size: 100px;" class="far fa-smile-beam" />
          Emotions
          
        </button>
      </a>
<!--Button for places-->
      <a id="places" href="/places">
        <button class="button">
          <i style="font-size: 100px;" class="fas fa-map-marker-alt" />
          Places
        </button>
      </a>
<!--Button for phrases-->
      <a id="phrases" href="/phrases">
        <button class="button"><i style="font-size: 100px;" class="far fa-comment"></i>Phrases</button>
      </a>
    </div>
  </div>

<!--button for food-->
  <div id="container3-5">
    <div id="vertical-center3-5">
      <a id="food" href="/food">
        <button class="button"><i style="font-size: 100px;" class="fas fa-apple-alt"></i>Food</button>
      </a>
<!--button for animals-->
      <a id="animals" href="/animals">
        <button class="button"><i style="font-size: 100px;" class="fas fa-dog"></i>Animals</button>
      </a>
    </div>
  </div>

</div>
