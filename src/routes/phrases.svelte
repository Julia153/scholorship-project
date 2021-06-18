<script>
  let hurtCounter = 0;
  let tiredCounter = 0;
  let thirstyCounter = 0;
  let bathroomCounter = 0;
  let helpCounter = 0;
  let hungryCounter = 0;
  //accessing the api library
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  //saying i am hurt
  function hurt() {
    hurtCounter++;
    if (hurtCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("I am hurt");
      window.speechSynthesis.speak(speech);
    } else {
      alert("Please only press the word buttons once, sometimes they take a second to speak")
      hurtCounter = 0
    }
  }

  //saying i need to use the bathroom
  function bathroom() {
    bathroomCounter++
    if (bathroomCounter <= 2) {
let speech = new SpeechSynthesisUtterance("I need to use the bathroom");
    window.speechSynthesis.speak(speech);
    } else {
      alert("Please only press the word buttons once, sometimes they take a second to speak");
      bathroomCounter = 0;
    }
    
  }

  //saying i need help
  function help() {
    helpCounter++
    if (helpCounter <= 2) {
let speech = new SpeechSynthesisUtterance("I need help");
    window.speechSynthesis.speak(speech);
    } else {
       alert("Please only press the word buttons once, sometimes they take a second to speak");
       helpCounter = 0;
    }
    
  }

  //saying i am hungry
  function hungry() {
    hungryCounter++
    if (hungryCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("I am hungry");
    window.speechSynthesis.speak(speech);
    } else {
      alert("Please only press the word buttons once, sometimes they take a second to speak");
      hungryCounter = 0;
    }
    
  }

  //saying i am thirsty
  function thirsty() {
    thirstyCounter ++

    if (thirstyCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("I am thirsty");
    window.speechSynthesis.speak(speech);
    } else {
      alert("Please only press the word buttons once, sometimes they take a second to speak");
      thirstyCounter = 0;
    }
    
  }

  //saying i am tired
  function tired() {
    tiredCounter++;

    if (tiredCounter <= 2) {
      let speech = new SpeechSynthesisUtterance("I am tired");
    window.speechSynthesis.speak(speech);
    } else {
      alert("Please only press the word buttons once, sometimes they take a second to speak");
      tiredCounter = 0;
    }
    
  }
</script>

<style>
  /* setting the height of the page and the background color*/
  #body {
    background-color: #80cddb;
    height: 800px;
  }

  /* setting the properties of the buttons */
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

  img {
    margin-left: 400px;
    height: 30%;
    width: auto;
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

  /* setting the size and color of the icons*/
  i {
    font-size: 100px;
    color: black;
  }
</style>

<div id="body">
  <!--Title-->
  <img src="phraseLogo.png" alt="phrases logo" />
  <!--linking the home button-->
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/home">
        <i style=" font-size: 100px; color: black;" class="fas fa-home" />
      </a>
    </div>
  </div>

  <div id="container">

    <!--I am tired button-->
    <button on:click={tired} class="button">
      <i class="fas fa-bed" />
      I am tired
    </button>
    <!--i am thirsty button-->
    <button on:click={thirsty} class="button">
      <i class="fas fa-glass-whiskey" />
      I am thirsty
    </button>
    <!--I am hungry button-->
    <button on:click={hungry} class="button">
      <i class="fas fa-utensils" />
      I am hungry
    </button>
    <!--i need help button-->
    <button on:click={help} class="button">
      <i class="far fa-life-ring" />
      I need help
    </button>
    <!--i am hurt button-->
    <button on:click={hurt} class="button">
      <i class="fas fa-ambulance" />
      I am hurt
    </button>
    <!--i need to use the bathroom button-->
    <button on:click={bathroom} class="button">
      <i class="fas fa-restroom" />
      I need to use the bathroom
    </button>
  </div>

</div>
