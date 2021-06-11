<script>
  //Accessing the api text to speech api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying frog
  function frog() {
    let speech = new SpeechSynthesisUtterance("frog");
    window.speechSynthesis.speak(speech);
  }

  //saying bird
  function bird() {
    let speech = new SpeechSynthesisUtterance("bird");
    window.speechSynthesis.speak(speech);
  }

  //saying dog
  function dog() {
    let speech = new SpeechSynthesisUtterance("Dog");
    window.speechSynthesis.speak(speech);
  }

  //saying cat
  function cat() {
    let speech = new SpeechSynthesisUtterance("Cat");
    window.speechSynthesis.speak(speech);
  }

  //saying fish
  function fish() {
    let speech = new SpeechSynthesisUtterance("Fish");
    window.speechSynthesis.speak(speech);
  }

  //saying horse
  function horse() {
    let speech = new SpeechSynthesisUtterance("Horse");
    window.speechSynthesis.speak(speech);
  }
</script>

<style>
  /* setting the height of the page and background color*/
  #body {
    background-color: #80cddb;
    height: 800px;
  }

  /* changing the buttons to look how i want them to from the bulma button class*/
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

  /* setting the placement of the home button*/
  #vertical-placement-home {
    margin: 0;
    position: relative;
    left: 10px;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  .button {
    display: flex;
    flex-direction: column;
  }

  i {
    font-size: 100px;
    color: black;
  }
</style>

<div id="body">
  <!--Title-->
  <h1 class="title">Animals</h1>
  <!--Home button-->
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/home">
        <i style=" font-size: 100px; color: black;" class="fas fa-home" />
      </a>
    </div>
  </div>

  <div id="container">

    <!--Rabbit button-->
    <div on:click={frog} class="button">
      <i class="fas fa-frog" />
      Frog
    </div>
    <!--horse button-->
    <div on:click={horse} class="button">
      <i class="fas fa-horse" />
      Horse
    </div>
    <!--fish button-->
    <div on:click={fish} class="button">
      <i class="fas fa-fish" />
      Fish
    </div>

    <!--dog button-->
    <div on:click={dog} class="button">
      <i class="fas fa-dog" />
      Dog
    </div>
    <!--cat button-->
    <div on:click={cat} class="button">
      <i class="fas fa-cat" />
      Cat
    </div>
    <!--bird button-->
    <div on:click={bird} class="button">
      <i class="fas fa-crow" />
      Bird
    </div>

  </div>

</div>
