


<!-- Imports -->


<!-- Script -->
<script>
  let openBracket = '{';
  let closeBracket = '}';
</script>

<!-- html -->
<div class='code-example-container'>
<h2>
  Try Zoic Cache!
</h2>
<section class='codeIntro' id='codeIntro'>
  <p>
    Using this library is a breeze.  Below we've included some snippets to show just how quickly you can be up and running with your caching layer.
    <br>
    Don't bog down your application with heavy boilerplate and definitely don't embed your caching logic into the application itself.  Require in Zoic, setup a few
    options and let Zoic handle all the caching logic for your RESTful API server-side caching needs.
  </p>
</section>

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
</div>

<style>

.code-example-container {
  background-color: #eeeeee;
  display: flex;
  flex-direction: column;
}

h2 {
 text-align: center;
}

.codeIntro {
  width: 30vw;
  height: 20vh;
  text-align: left;
  position: relative;
  display:flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: stretch;
  margin:auto
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