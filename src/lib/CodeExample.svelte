


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
          <span style="color:#9cdcfe">Zoic</span>
          <span style="color:yellow">{@html closeBracket}</span>
          <span style="color:#ae81ff"> from </span>
          <span style="color:orange">{@html '../../OSP/zoic.ts'}</span><span style="color:white">;</span>
        </span>
      </span>
      <br> 
      <span style="display:flex"> 
        <span>
          <span>
            <span style="color:#9cdcfe">router</span><span style="color:white">.</span><span style="color:yellow">get</span><span style="color:yellow">{@html '('}</span><!--
            --><span style="color:orange">{@html "'/endpoint'"}</span><!--
            --><span style="color:white">,</span>
            <span style="color:#9cdcfe">zoic.use</span><!--
            --><span style="color:white">,</span>
            <span style="color:#9cdcfe">controller.dbRead</span><!--
            --><span style="color:yellow">{@html ')'}</span>
          </span>
        </span>
      </span>
    </code>
  </div>

  <div class='codeIntroContainer' id='codeIntro'>
    <div class="codeIntroTitle">
      <i>
        Try Zoic Cache!
      </i>
    </div>

    <div class='codeIntroBody'><p>
      A caching middleware library for Oak
      <br><br>
      Using this library is a breeze.  Below we've included some snippets to show just how quickly you can be up and running with your caching layer.
      <br><br>
      Don't bog down your application with heavy boilerplate and definitely don't embed your caching logic into the application itself.  Require in Zoic, setup a few
      options and let Zoic handle all the caching logic for your RESTful API server-side caching needs.<br><br>
      <button><span class="button_top" href="#">Download it here</span></button>
    </p>
    </div>
  </div>

</div>

<style>

.code-example-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  padding: 50px;
  justify-content: space-evenly;  
  /* flex-direction: column; */

} 

.code-block-container {
  /* display: flex; */
  /* position: relative; */
  flex-direction: column;
  justify-content: space-evenly;
  /* align-items: stretch; */
  margin: auto;
  padding: 25px;
  font-size: 1.4rem;
  /* width: 35vw;
  height: 20vh; */
  background-color:#272822;
  border-radius: 30px;
  /* min-width: 200px; */
  width:600px;
  box-shadow: 10px 5px 5px rgb(127, 124, 124);

}

.codeIntroContainer {
  width: 35vw;
  padding: 5em;
  text-align: right;
  /* min-width: 200px; */
}


.codeIntroTitle {
  font-size: 3em;
  color: white;
  text-shadow: 2px 2px 4px;
  /* text-align: right; */
}

.codeIntroBody {
  font-size: 1.5em;
  color: white;
}



/* .codeIntro {
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
} */

/* button {
  color: blue;
  font-size: .75em;
  background: lightblue;
  width: 10em;
  height: 1.8em;

} */
/* From uiverse.io by @Voxybuns */

button {
  /* Variables */
 --button_radius: 0.75em;
 --button_color: #e8e8e8;
 --button_outline_color: #000000;
 font-size: 17px;
 font-weight: bold;
 border: none;
 border-radius: var(--button_radius);
 background: var(--button_outline_color);
}

.button_top {
 display: block;
 box-sizing: border-box;
 border: 2px solid var(--button_outline_color);
 border-radius: var(--button_radius);
 padding: 0.75em 1.5em;
 background: var(--button_color);
 color: var(--button_outline_color);
 transform: translateY(-0.2em);
 transition: transform 0.1s ease;
}

button:hover .button_top {
  /* Pull the button upwards when hovered */
 transform: translateY(-0.33em);
}

button:active .button_top {
  /* Push the button downwards when pressed */
 transform: translateY(0);
}

@media screen and (max-width: 1450px) {
  .codeIntroContainer {
    text-align: center;
  }
}



</style>