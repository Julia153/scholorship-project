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

  /* setting buttons to be in a row*/
  #container1 {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-left: 100px;
  }
  /* setting buttons to be in a row*/
  #container2 {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-left: 100px;
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

  .button {
    display: flex;
    flex-direction: column;
  }

  #animalsIcon {
    margin-left: 30px;
  }

  #emotionsIcon {
    margin-right: 40px;
    margin-top: 10px;
  }

  #placesIcon {
    margin-left: 20px;
  }

  #foodIcon {
    margin-left: 20px;
    width: 80%;
    height: auto;
  }

</style>

<!--Div for whole page to set background color-->
<div id="body">
  <!--Setting my title to be my SkyShip logo-->
  <h1 class="title">
    <img
      style="height: 30%; width: auto; margin: 0px;"
      src="SkyShipLogo.png"
      alt="SkyShip title words sky ship in clouds with a rocket launching" />
  </h1>
  <!--Button to logout-->
  <a id="logOutLink" href="/">Log In</a>
  <!--Button to go to settings-->
  <a id="settingsLink" href="/settings">Settings</a>

  <!--Buttons for emotions-->
  <div id="container1">

    <a id="emotions" href="/emotions">
      <div class="button">
        <img id="emotionsIcon" src="emotions.png" alt="emotions icon">
        Emotions
      </div>
    </a>
    <!--Button for places-->
    <a id="places" href="/places">
      <div class="button">
        <img id="placesIcon" src="places.png" alt="Places icon">
        Places
      </div>
    </a>
    <!--Button for phrases-->
    <a id="phrases" href="/phrases">
      <div class="button">
        <img src="phrases.png" alt="phrases icon">
        Phrases
      </div>
    </a>

    <div id="container2">

      <!--button for food-->

      <a id="food" href="/food">
        <div class="button">
          <img id="foodIcon" src="food.png" alt="food icon">
          Food
        </div>
      </a>
      <!--button for animals-->
      <a id="animals" href="/animals">
        <div class="button">
          <img id="animalsIcon" src="animals.png" alt="animals icon">
          Animals
        </div>
      </a>
    </div>
  </div>

</div>
