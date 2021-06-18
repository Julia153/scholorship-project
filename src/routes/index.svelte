<script>
  // create an empty person object
  let person = {
    firstName: "",
    lastName: "",
    age: ""
  };

  function savePerson() {
    console.log("savePerson() clicked");
    // save the person object to the database under their first name

    db.collection("People")
      .doc(person.firstName)
      .set(person);
  }

  async function getPerson() {
    // get the document from the database for the given name
    let personDoc = await db
      .collection("People")
      .doc(person.firstName)
      .get();

    // get the data from the person document
    person = personDoc.data();
  }
  
</script>

<style>
  /* making the title centered*/
  h1 {
    text-align: center;
  }

  /* setting the button properties for the button to use without logging in*/
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

  /* setting spacing between the buttons*/
  .button {
    margin: 30px;
  }

  /* setting the sign in buttons in columns*/
  .container {
    display: flex;
    flex-direction: column;
    float: right;
    margin-right: 300px;
    margin-top: 30px;
  }

  /*  setting the properties of the sing in buttons*/
  #google,
  #apple,
  #microsoft {
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
<!--use without logging in button-->
<a href="/home">
  <button id="noLogIn" class="button">Use without logging in</button>
</a>


<!-- this is just a section to make the page look nice -->
<section class="content section">

  <h1>People</h1>

  <!-- a place to enter the first name -->
  <label>
    First name:
    <input bind:value={person.firstName} />
  </label>

  <!-- a place to enter the last name -->
  <label>
    Last name:
    <input bind:value={person.lastName} />
  </label>

  <!-- a place to enter the age -->
  <label>
    Age:
    <input bind:value={person.age} />
  </label>

  <button on:click={getPerson}>Get Person</button>

  <button on:click={savePerson}>Save Person</button>

</section>

<div class="container">
  <!--log in with google button-->
  <button id="google" class="button">Log in with Google</button>
  <!-- log in with microsoft button-->
  <button id="microsoft" class="button">Log in with Microsoft</button>
  <!--log in with apple button-->
  <button id="apple" class="button">Log in with Apple</button>
</div>
