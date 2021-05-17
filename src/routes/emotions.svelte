<script>
let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function frustrated() {
    let speech = new SpeechSynthesisUtterance('frustrated');
    window.speechSynthesis.speak(speech);
  }

  function scared() {
    let speech = new SpeechSynthesisUtterance('scared');
    window.speechSynthesis.speak(speech);
  }

  function sad() {
    let speech = new SpeechSynthesisUtterance('sad');
    window.speechSynthesis.speak(speech);
  }
 
  function happy() {
    let speech = new SpeechSynthesisUtterance('happy');
    window.speechSynthesis.speak(speech);
  }

  function excited() {
    let speech = new SpeechSynthesisUtterance('excited');
    window.speechSynthesis.speak(speech);
  }

  function angry() {
    let speech = new SpeechSynthesisUtterance('angry');
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
  <h1 class="title">Emotions</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <img id="homeIcon" src="home.png" alt="home icon" />
      </a>
    </div>
  </div>

  <div id="container1">
    <div id="vertical-center1">
      <button id="water" on:click={happy} class="button">Happy</button>
      <button id="juice" on:click={sad} class="button">Sad</button>
      <button id="milk" on:click={angry} class="button">Angry</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="chicken" on:click={frustrated} class="button">Frustrated</button>
      <button id="apple" on:click={excited} class="button">Excited</button>
      <button id="cracker" on:click={scared} class="button">Scared</button>
    </div>
  </div>

</div>
