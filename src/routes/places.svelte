<script>
let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function school() {
    let speech = new SpeechSynthesisUtterance('school');
    window.speechSynthesis.speak(speech);
  }

  function museum() {
    let speech = new SpeechSynthesisUtterance('museum');
    window.speechSynthesis.speak(speech);
  }

  function pool() {
    let speech = new SpeechSynthesisUtterance('pool');
    window.speechSynthesis.speak(speech);
  }
 
  function grandparents() {
    let speech = new SpeechSynthesisUtterance('grandparents House');
    window.speechSynthesis.speak(speech);
  }

  function home() {
    let speech = new SpeechSynthesisUtterance('home');
    window.speechSynthesis.speak(speech);
  }

  function park() {
    let speech = new SpeechSynthesisUtterance('park');
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

  #vertical-placement-home {
    margin: 0;
    position: relative;
    left: 10px;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }
  
</style>

<div id="body">
  <h1 class="title">Places</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <img id="homeIcon" src="home.png" alt="home icon" />
      </a>
    </div>
  </div>

  <div id="container1">
    <div id="vertical-center1">
      <button id="water" on:click={home} class="button">Home</button>
      <button id="juice" on:click={park} class="button">Park</button>
      <button id="milk" on:click={school} class="button">School</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="chicken" on:click={grandparents} class="button">Grandparents house</button>
      <button id="apple" on:click={museum} class="button">Museum</button>
      <button id="cracker" on:click={pool} class="button">Pool</button>
    </div>
  </div>

</div>
