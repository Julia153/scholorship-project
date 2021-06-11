<script>
  //accessing the api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying school
  function school() {
    let speech = new SpeechSynthesisUtterance("school");
    window.speechSynthesis.speak(speech);
  }

  //saying zoo
  function zoo() {
    let speech = new SpeechSynthesisUtterance("zoo");
    window.speechSynthesis.speak(speech);
  }

  //saying pool

  function pool() {
    let speech = new SpeechSynthesisUtterance("pool");
    window.speechSynthesis.speak(speech);
  }

  //saying playground
  function playground() {
    let speech = new SpeechSynthesisUtterance("playground");
    window.speechSynthesis.speak(speech);
  }

  //saying home
  function home() {
    let speech = new SpeechSynthesisUtterance("home");
    window.speechSynthesis.speak(speech);
  }

  //saying park
  function park() {
    let speech = new SpeechSynthesisUtterance("park");
    window.speechSynthesis.speak(speech);
  }
</script>

<style>
  /* setting the height of the page and the background color*/
  #body {
    background-color: #80cddb;
    height: 800px;
  }

  /* setting the button properties*/
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

  /* setting the placement of the home button*/
  #vertical-placement-home {
    margin: 0;
    position: relative;
    left: 10px;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  img {
    height: 50%;
    width: auto;
  }

  i {
    font-size: 100px;
    color: black;
  }
</style>

<div id="body">
  <!--title-->
  <h1 class="title">Places</h1>
  <!--home button-->
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/home">
        <i style="font-size: 100px; color: black;" class="fas fa-home"></i>
      </a>
    </div>
  </div>

  <div id="container">
    <!--home button-->
    <div on:click={home} class="button">
      <i  id="homePlace" class="fas fa-home"></i>
      Home
    </div>
    <!--park button-->
    <div on:click={park} class="button">
      <i class="fas fa-tree" />
      Park
    </div>
    <!--school button-->
    <div on:click={school} class="button">
      <i class="fas fa-school" />
      School
    </div>
    <!--playground button-->
    <div on:click={playground} class="button">
      <img src="swing.png" alt="swing">
      Playground
    </div>
    <!--zoo button-->
    <div on:click={zoo} class="button">
      <i class="fas fa-hippo"></i>
      Zoo
    </div>
    <!--pool buttonÏ-->
    <div on:click={pool} class="button">
      <i class="fas fa-swimming-pool" />
      Pool
    </div>

  </div>

</div>
