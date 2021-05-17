<script>
let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function hurt() {
    let speech = new SpeechSynthesisUtterance('I am hurt');
    window.speechSynthesis.speak(speech);
  }

  function bathroom() {
    let speech = new SpeechSynthesisUtterance('I need to use the bathroom');
    window.speechSynthesis.speak(speech);
  }

  function help() {
    let speech = new SpeechSynthesisUtterance('I need help');
    window.speechSynthesis.speak(speech);
  }
 
  function hungry() {
    let speech = new SpeechSynthesisUtterance('I am hungry');
    window.speechSynthesis.speak(speech);
  }

  function thirsty() {
    let speech = new SpeechSynthesisUtterance('I am thirsty');
    window.speechSynthesis.speak(speech);
  }

  function tired() {
    let speech = new SpeechSynthesisUtterance('I am tired');
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
  <h1 class="title">Phrases</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <img id="homeIcon" src="home.png" alt="home icon" />
      </a>
    </div>
  </div>

  <div id="container1">
    <div id="vertical-center1">
      <button id="water" on:click={tired} class="button">I am tired</button>
      <button id="juice" on:click={thirsty} class="button">I am thirsty</button>
      <button id="chicken" on:click={hungry} class="button">I am hungry</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="milk" on:click={help} class="button">I need help</button>
      <button id="apple" on:click={hurt} class="button">I am hurt</button>
      <button id="cracker" on:click={bathroom} class="button">I need to use the bathroom</button>
    </div>
  </div>

</div>
