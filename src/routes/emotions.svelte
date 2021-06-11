<script>
  //accessing the api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying frustrated
  function frustrated() {
    let speech = new SpeechSynthesisUtterance("frustrated");
    window.speechSynthesis.speak(speech);
  }

  //saying scared
  function scared() {
    let speech = new SpeechSynthesisUtterance("scared");
    window.speechSynthesis.speak(speech);
  }

  //saying sad
  function sad() {
    let speech = new SpeechSynthesisUtterance("sad");
    window.speechSynthesis.speak(speech);
  }

  //saying happy
  function happy() {
    let speech = new SpeechSynthesisUtterance("happy");
    window.speechSynthesis.speak(speech);
  }

  //saying excited
  function excited() {
    let speech = new SpeechSynthesisUtterance("excited");
    window.speechSynthesis.speak(speech);
  }

  //saying angry
  function angry() {
    let speech = new SpeechSynthesisUtterance("angry");
    window.speechSynthesis.speak(speech);
  }
</script>

<style>
  /* setting the height of the page and the background color*/
  #body {
    background-color: #80cddb;
    height: 800px;
  }

  /* setting the button properties for how i want it to look chaning it from the bulma button class*/
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

  /* setting the placement of the home button*/
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

  /* centering the word buttons*/
  #container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    margin-left: 100px;
  }
</style>

<div id="body">
  <!--title-->
  <h1 class="title">Emotions</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <!--home button-->
      <a href="/home">
        <i style=" font-size: 100px; color: black;" class="fas fa-home" />
      </a>
    </div>
  </div>

  <div id="container">
    <!--happy button-->
    <div on:click={happy} class="button">
      <i class="far fa-smile" />
      Happy
    </div>
    <!--sad button-->
    <div on:click={sad} class="button">
      <i class="far fa-sad-tear" />
      Sad
    </div>
    <!--angry button-->
    <div on:click={angry} class="button">
      <i class="far fa-angry" />
      Angry
    </div>
    <!--frustrated button-->
    <div on:click={frustrated} class="button">
      <i class="far fa-tired" />
      Frustrated
    </div>
    <!--excited button-->
    <div on:click={excited} class="button">
      <i class="far fa-laugh-squint" />
      Excited
      <!--scared button-->
    </div>
    <div on:click={scared} class="button">
      <i class="far fa-flushed" />
      Scared
    </div>
  </div>

</div>
