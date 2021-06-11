<script>
  //accessing the api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying pizza

  function pizza() {
    let speech = new SpeechSynthesisUtterance("pizza");
    window.speechSynthesis.speak(speech);
  }

  //saying apple
  function apple() {
    let speech = new SpeechSynthesisUtterance("apple");
    window.speechSynthesis.speak(speech);
  }

  //saying water
  function water() {
    let speech = new SpeechSynthesisUtterance("water");
    window.speechSynthesis.speak(speech);
  }

  //saying carrot
  function carrot() {
    let speech = new SpeechSynthesisUtterance("carrot");
    window.speechSynthesis.speak(speech);
  }

  //saying egg
  function egg() {
    let speech = new SpeechSynthesisUtterance("egg");
    window.speechSynthesis.speak(speech);
  }

  //saying cake
  function cake() {
    let speech = new SpeechSynthesisUtterance("cake");
    window.speechSynthesis.speak(speech);
  }
</script>

<style>
  /* setting height of page and background color*/
  #body {
    background-color: #80cddb;
    height: 800px;
  }

  /* editing the button properties from the bulma button class*/
  .button {
    width: 300px;
    height: 300px;
    margin: 20px;
    border-style: solid;
    border-width: 10px;
    border-color: #1d3461;
    border-radius: 10px;
    background-color: #f5f6f4;
    display: flex;
    flex-direction: column;
  }

  /* making the title image centered*/
  .title {
    text-align: center;
  }

  /* centering the word buttons*/
  #container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-left: 100px;
  }

  /* placement of the home button*/
  #vertical-placement-home {
    margin: 0;
    position: relative;
    left: 10px;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  i {
    font-size: 100px;
    color: black;
  }

</style>

<div id="body">
  <!--title-->
  <h1 class="title">Food and Drinks</h1>
  <!-- home button -->
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/home">
        <i style=" font-size: 100px; color: black;" class="fas fa-home" />
      </a>
    </div>
  </div>

  <div id="container">
    <!--water button-->
    <button on:click={water} class="button">
      <i class="fas fa-tint"></i>
      Water
    </button>
    <!--pizza button-->
    <button on:click={pizza} class="button">
     <i class="fas fa-pizza-slice"></i>
      Pizza
    </button>
    <!--egg button-->
    <button on:click={egg} class="button">
      <i class="fas fa-egg"></i>
      Egg
    </button>

    <!--carrot button-->
    <button on:click={carrot} class="button">
      <i class="fas fa-carrot"></i>
      Carrot
    </button>

    <!--apple button-->
    <button on:click={apple} class="button">
      <i class="fas fa-apple-alt"></i>
      Apple
    </button>

    <!--cake button-->
    <button id="cake" on:click={cake} class="button">
      <i class="fas fa-birthday-cake"></i>
      Cake
    </button>

  </div>

</div>
