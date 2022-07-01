<script>

</script>
<div class="devtoolBox">
  <span>
    <div class="devtoolGif">
      <img src='../public/images/tempGif.gif' alt="Zoic chrome extension demo" />
    </div>

  </span>
  <div class="devtoolText">
    <div class="devtoolTitle">
       <i>DevTools</i> 
    </div>
    <p>
      The Zoic Developer Tool is a Chrome Developer Tools extension for monitoring metrics in a ZoicCache instance. With Zoic Developer Tool, you can monitor and inspect memory usage, reads processed, writes proccesed, latency, and more.
      <br><br>
      <button>
        <span href="" class="button_top">
          Download it here!    
        </span>
      </button>
    </p>
  </div>

</div>
  
<style>

  div {
    color: white;
    justify-content: space-around;
    /* background-color: #E0BB76; */
  }
  .devtoolTitle {
    font-size: 2.3em;
    text-shadow: 2px 2px 4px #fffbf3;
  }

  .devtoolBox {
    padding: 50px;
    border-color: #E0BB76;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    padding-top: 150px;
  }

  .devtoolText {
    color: white;
    width: 50%;
    margin-right: 50px; 
    text-align: right;
    font-size: 1.5rem;
    margin-left: 30px;
  }

  img {
    width: 600px;
    border-radius: 30px;
  }

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

img {
      border: 2px solid rgb(53, 47, 47);
      box-shadow: 10px 5px 5px rgb(127, 124, 124);

    }

  @media screen and (max-width: 1475px) {
    .devtoolText {
    text-align: center;
  }
}
</style>