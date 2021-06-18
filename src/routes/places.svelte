<script>
  let homePlaceCounter = 0;
  let parkCounter = 0;
  let schoolCounter = 0;
  let playgroundCounter = 0;
  let zooCounter = 0;
  let poolCounter = 0;

  //accessing the api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying school
  function school() {
    schoolCounter++;
    if (schoolCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("school");
      window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      schoolCounter = 0;
    }
  }

  //saying zoo
  function zoo() {
    zooCounter++;
    if (zooCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("zoo");
      window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      zooCounter = 0;
    }
  }

  //saying pool

  function pool() {
    poolCounter ++
    if (poolCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("pool");
      window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      poolCounter = 0;
    }
  }

  //saying playground
  function playground() {
    playgroundCounter++;
    if (playgroundCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("playground");
      window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      playgroundCounter = 0;
    }
  }

  //saying home
  function homePlace() {
    homePlaceCounter++
    if (homePlaceCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("home");
    window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      homePlaceCounter = 0;
    }
    
  }

  //saying park
  function park() {
    parkCounter++
    if (parkCounter <= 2) {
let speech = new SpeechSynthesisUtterance("park");
    window.speechSynthesis.speak(speech);
    } else {
      alert(
        "Please only press the button once, sometimes it takes a second for the word to speak"
      );
      parkCounter = 0;
    }
    
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

  #body {
    height: 1100px;
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

  i {
    font-size: 100px;
    color: black;
  }
</style>

<div id="body">
  <!--title-->
  <img
    style="margin-left: 400px; height: 30%; width: auto;"
    src="placeLogo.png"
    alt="places logo" />
  <!--home button-->
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/home">
        <i style="font-size: 100px; color: black;" class="fas fa-home" />
      </a>
    </div>
  </div>

  <div id="container">
    <!--home button-->
    <div on:click={homePlace} class="button">
      <i id="homePlace" class="fas fa-home" />
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
      <img style="height: 50%; width: auto;" src="swing.png" alt="swing" />
      Playground
    </div>
    <!--zoo button-->
    <div on:click={zoo} class="button">
      <i class="fas fa-hippo" />
      Zoo
    </div>
    <!--pool buttonÏ-->
    <div on:click={pool} class="button">
      <i class="fas fa-swimming-pool" />
      Pool
    </div>

  </div>

</div>
