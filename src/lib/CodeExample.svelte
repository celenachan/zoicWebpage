


<!-- Imports -->


<!-- Script -->
<script>
  let openBracket = '{';
  let closeBracket = '}';
</script>

<!-- html -->
<div class='code-example-container'>

<div class='code-block-container' id='code-block-container'>
  <code class="language-typescript" data-lang="typescript">
    <span style="display:flex">
      <span>
        <span style="color:#ae81ff">import </span>
        <span style="color:yellow">{@html openBracket}</span>
        <span style="color:#5d5dae"> Zoic </span>
        <span style="color:yellow">{@html closeBracket}</span>
        let tryZoic = true;
      </span>
    </span>
    let test = '';
  </code>
</div>
<div class='codeIntro' id='codeIntro'>
  <div class="codeIntroTitle">
    <i>Try Zoic Cache!</i>
  </div>

  <div class='codeIntroBody'><h2>
    Using this library is a breeze.  Below we've included some snippets to show just how quickly you can be up and running with your caching layer.
    <br>
    Don't bog down your application with heavy boilerplate and definitely don't embed your caching logic into the application itself.  Require in Zoic, setup a few
    options and let Zoic handle all the caching logic for your RESTful API server-side caching needs.
    </h2>
  </div>
</div>

</div>

<style>

.code-example-container {
  /* background-color: #EE892F; */
  display: flex;
  padding: 100px;
  justify-content: space-around;
  /* flex-direction: column; */
}

h2 {
  text-align: center;
}

.codeIntroTitle {
  font-size: 100px;
  color: white;
  text-shadow: 2px 2px 4px;
  /* text-align: right; */
}
.codeIntroBody {
  font-size: 1fr;
}

.codeIntro {
  width: 50vw;
  height: 20vh;
  text-align:right;
  position: relative;
  display:flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: stretch;
  margin:auto;
  color: white;
}

.code-block-container {
  display: flex;
  position: relative;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: stretch;
  margin: auto;
  width: 20vw;
  height: 20vh;
  background-color:#272822;
}

</style>