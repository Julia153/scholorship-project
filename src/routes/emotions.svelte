<script>
  let speech = new SpeechSynthesisUtterance();
  speech.lang = "en";

  function frustrated() {
    let speech = new SpeechSynthesisUtterance("frustrated");
    window.speechSynthesis.speak(speech);
  }

  function scared() {
    let speech = new SpeechSynthesisUtterance("scared");
    window.speechSynthesis.speak(speech);
  }

  function sad() {
    let speech = new SpeechSynthesisUtterance("sad");
    window.speechSynthesis.speak(speech);
  }

  function happy() {
    let speech = new SpeechSynthesisUtterance("happy");
    window.speechSynthesis.speak(speech);
  }

  function excited() {
    let speech = new SpeechSynthesisUtterance("excited");
    window.speechSynthesis.speak(speech);
  }

  function angry() {
    let speech = new SpeechSynthesisUtterance("angry");
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

  #vertical-placement-home {
    margin: 0;
    position: relative;
    left: 10px;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin-left: 100px;
}
</style>

<div id="body">
  <h1 class="title">Emotions</h1>
  <div id="homeContainer">
    <div id="vertical-placement-home">
      <a href="/">
        <i style=" font-size: 100px; color: #1D3461;" class="fas fa-home"></i>
      </a>
    </div>
  </div>

  <div id="container">
    <div id="happy" on:click={happy} class="button"><i style="font-size: 50px; margin: 10px;" class="far fa-smile"></i>Happy</div>
    <div id="sad" on:click={sad} class="button"><i style="font-size: 50px; margin: 10px;"class="far fa-sad-tear"></i>Sad</div>
    <div id="angry" on:click={angry} class="button"><i style="font-size: 50px; margin: 10px;"class="far fa-angry"></i>Angry</div>
    <div id="frustrated" on:click={frustrated} class="button"><i style="font-size: 50px; margin: 10px;"class="far fa-tired"></i>Frustrated</div>
    <div id="excited" on:click={excited} class="button">
      <i style="font-size: 50px; margin: 10px;" class="far fa-laugh-squint" />
      Excited
    </div>
    <div id="scared" on:click={scared} class="button"><i style="font-size: 50px; margin: 10px;"class="far fa-flushed"></i>Scared</div>
  </div>

</div>
