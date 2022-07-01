<script>
  import { onMount } from "svelte";

  export let navItems = [];

  function scrollIntoView({ target }) {
		const el = document.querySelector(target.getAttribute('href'));
		if (!el) return;
    el.scrollIntoView({
      behavior: 'smooth'
    });
  }

</script>

<div class='imgAndNavContainer'>
    <nav>
      <div class="navBar">
        <ul class="navbar-list">
          {#each navItems as item}
            <a href={item.href}>{item.label}</a>
          {/each}
        </ul>
      </div>
    </nav>
    <div class='imgContainer'>
      <a href="#introLink" id="scrollButton" on:click|preventDefault={scrollIntoView}>find out more</a>
      <img id='dinoImg' src="../public/images/zoic_new.png" alt='large, plant eating dinosaur in a river'>
    </div>
    <div class='separationDivI'>
    </div>
    <div class='separationDivII'>
    </div>
</div>

<style>

.imgContainer #scrollButton {
  position: absolute;
  color: white;
  top:80%;
  left: 50%;
  box-sizing: border-box;
  height: 5vw;
  width: 5vw;
  border-style: solid;
  border-color: white;
  border-width: 0px 1px 1px 0px;
  transform: rotate(45deg);
  transition: border-width 150ms ease-in-out;

  /* background-image: linear-gradient(#2e475d, 90%, transparent); */
  /* overflow: hidden; */
}

.separationDivI {
    background-color: #2E485D;
    height: 30px;
    margin: -5px;
}

.separationDivII {
    background-image: linear-gradient(#2E485D, 80%, transparent);
    height: 30px;
    margin: -5px;
}

/* #scrollButton {
  color:white;
  position: center;
} */
/* .blur {
  margin-bottom: -1px;
  filter: blur(10px);
  width: 100%;
  height: 10px;
  margin: -10px;
} */


  nav {
    background-color: rgba(0, 0, 0, 0.8);
    font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
    height: 45px;
    width: 100vw;
    position: fixed;
    z-index: 10;
    opacity: 90%;
    background: linear-gradient(to right, transparent, 75%, rgb(27, 23, 23));
    font-size: medium;

    /* Fade in  */
    -webkit-animation: fadein 2.5s; /* Safari, Chrome and Opera > 12.1 */
       -moz-animation: fadein 2.5s; /* Firefox < 16 */
        -ms-animation: fadein 2.5s; /* Internet Explorer */
         -o-animation: fadein 2.5s; /* Opera < 12.1 */
            animation: fadein 2.5s;
  }

 

@keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}

/* Firefox < 16 */
@-moz-keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}

/* Safari, Chrome and Opera > 12.1 */
@-webkit-keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
}


  .navbar-list {
    display: none;
    margin: 0;
    padding: 0 40px;
    justify-content: flex-end;

  }

      .navbar-list a {
        color: white;
        font-weight: bold;
        height: 45px;
        display: flex;
        align-items: center;
        padding: 0 10px;
        font-size: 13px;
        margin: 0 10px;
        font-size: 1em;

      }

    .navbar-list {
      display: flex;
    }

    .navbar-list a {
      display: inline-flex;
      padding: 0;
    }

  #dinoImg {
    width: 100vw;
    height: 100vh;
}

a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  /* text-decoration: underline; */
  border-bottom-width: 4px;
  border-right-width: 4px;
}

a:active {
  text-decoration: underline;
}




    
  </style>
