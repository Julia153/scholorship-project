<script>
let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function rabbit() {
    let speech = new SpeechSynthesisUtterance('rabbit');
    window.speechSynthesis.speak(speech);
  }

  function bird() {
    let speech = new SpeechSynthesisUtterance('bird');
    window.speechSynthesis.speak(speech);
  }

  function dog() {
    let speech = new SpeechSynthesisUtterance('Dog');
    window.speechSynthesis.speak(speech);
  }
 
  function cat() {
    let speech = new SpeechSynthesisUtterance('Cat');
    window.speechSynthesis.speak(speech);
  }

  function fish() {
    let speech = new SpeechSynthesisUtterance('Fish');
    window.speechSynthesis.speak(speech);
  }

  function horse() {
    let speech = new SpeechSynthesisUtterance('Horse');
    window.speechSynthesis.speak(speech);
  }
</script>

<style>
  #body {
    background-color: #80cddb;
    height: 800px;
  }

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

  .title {
    text-align: center;
  }

  #container1 {
    height: 200px;
    position: relative;
  }

  #vertical-center1 {
    margin: 0;
    position: absolute;
    right: 10%;
    top: 80%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #container2 {
    height: 200px;
    position: relative;
  }

  #vertical-center2 {
    margin: 0;
    position: absolute;
    right: 10%;
    top: 150%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #homeIcon {
    width: 10%;
    height: 10%;
  }
</style>

<div id="body">
  <h1 class="title">Animals</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <img id="homeIcon" src="home.png" alt="home icon" />
      </a>
    </div>
  </div>

  <div id="container1">
    <div id="vertical-center1">
      <button id="water" on:click={rabbit} class="button">Rabbit</button>
      <button id="juice" on:click={horse} class="button">Horse</button>
      <button id="chicken" on:click={fish} class="button">Fish</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="milk" on:click={dog} class="button">Dog</button>
      <button id="apple" on:click={cat} class="button">Cat</button>
      <button id="cracker" on:click={bird} class="button">Bird</button>
    </div>
  </div>

</div>
