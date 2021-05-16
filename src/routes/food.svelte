<script>
  let speech = new SpeechSynthesisUtterance();
speech.lang = "en";

function chicken() {
  let speech = new SpeechSynthesisUtterance('chicken');
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
      <button id="water" class="button">Water</button>
      <button id="juice" class="button">Juice</button>
      <button id="milk" class="button">Milk</button>
    </div>
  </div>
  <div id="container2">
    <div id="vertical-center2">
      <button id="chicken" on:click={chicken} class="button">Chicken</button>
      <button id="apple" class="button">Apple</button>
      <button id="cracker" class="button">Cracker</button>
    </div>
  </div>

  
</div>
