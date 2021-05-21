<style>

h1 {
    text-align: center;
}

#noLogIn {
    width: 500px;
    height: 500px;
    margin: 20px;
    border-style: solid;
    border-width: 10px;
    border-color: #1d3461;
    border-radius: 10px;
    background-color: #f5f6f4;
    font-size: 40px;
  }

.button {
    margin: 30px;
}
.container {
    display: flex;
  flex-direction: column;
  float: right; 
  margin-right: 300px;
  margin-top: 30px;
}

#google, #apple, #microsoft {
    height: 100px;
    width: 300px;
    border-style: solid;
    border-width: 8px;
    border-color: #1d3461;
    border-radius: 10px;
    background-color: #f5f6f4;
}




</style>

<h1 class="title">SkyShip</h1>
<a href="/">
    <button id="noLogIn" class="button">Use without logging in</button>
</a>


<div class="container">
<button id="google" class="button">Log in with Google</button>
<button id="microsoft" class="button">Log in with Microsoft</button>
<button id="apple" class="button">Log in with Apple</button>
</div>



