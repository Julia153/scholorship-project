<script>
let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function chicken() {
    let speech = new SpeechSynthesisUtterance('chicken');
    window.speechSynthesis.speak(speech);
  }

  function apple() {
    let speech = new SpeechSynthesisUtterance('apple');
    window.speechSynthesis.speak(speech);
  }

  function water() {
    let speech = new SpeechSynthesisUtterance('water');
    window.speechSynthesis.speak(speech);
  }
 
  function juice() {
    let speech = new SpeechSynthesisUtterance('juice');
    window.speechSynthesis.speak(speech);
  }

  function milk() {
    let speech = new SpeechSynthesisUtterance('milk');
    window.speechSynthesis.speak(speech);
  }

  function cracker() {
    let speech = new SpeechSynthesisUtterance('cracker');
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
  
  i {
    font-size: 50px;
  }
</style>

<div id="body">
  <h1 class="title">Food and Drinks</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <img id="homeIcon" src="home.png" alt="home icon" />
      </a>
    </div>
  </div>

  <div id="container1">
    <div id="vertical-center1">
      <button id="water" on:click={water} class="button"><img style="height: 50%; width: auto;"src="water-bottle.png" alt="water bottle" Water>Water</button>
      <button id="juice" on:click={juice} class="button"><img style="height: 50%; width: auto;"src="juice.png" alt="juice">Juice</button>
      <button id="milk" on:click={milk} class="button"><img style="height: 50%; width: auto;" src="milk.png" alt="milk">Milk</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="chicken" on:click={chicken} class="button"><i class="fas fa-drumstick-bite"></i>Chicken</button>
      <button id="apple" on:click={apple} class="button"><i class="fas fa-apple-alt"></i>Apple</button>
      <button id="cracker" on:click={cracker} class="button"><img style="height: 50%; width: auto;"src="cracker.png" alt="cracker">Cracker</button>
    </div>
  </div>

</div>
