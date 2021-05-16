<script>

</script>

<style>
  .title {
    text-align: center;
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

  #container1-3 {
    height: 200px;
    position: relative;
  }

  #vertical-center1-3 {
    margin: 0;
    position: absolute;
    right: 10%;
    top: 80%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #container3-5 {
    height: 200px;
    position: relative;
  }

  #vertical-center3-5 {
    margin: 0;
    position: absolute;
    right: 24%;
    top: 150%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
  }

  #body {
      background-color: #80CDDB;
      height: 800px;
  }
</style>

<div id="body">
  <h1 class="title">Name of Website goes here</h1>

  <div id="container1-3">
    <div id="vertical-center1-3">
      <a id="emotions" href="/emotions">
        <button class="button">Emotions<i class="far fa-smile-beam"></i></button>
      </a>

      <a id="places" href="/places">
        <button class="button">Places</button>
      </a>

      <a id="phrases" href="/phrases">
        <button class="button">Phrases</button>
      </a>
    </div>
  </div>

  <div id="container3-5">
    <div id="vertical-center3-5">
      <a id="food" href="/food">
        <button class="button">Food</button>
      </a>

      <a id="animals" href="/animals">
        <button class="button">Animals</button>
      </a>
    </div>
  </div>

</div>
