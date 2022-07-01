<script>
  import { onMount } from "svelte";

  export let navItems = [];

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
      <img id='dinoImg' src="https://cdn.cnn.com/cnnnext/dam/assets/220209135129-01-dinosaur-respiratory-infection-exlarge-169.jpg" alt='large, plant eating dinosaur in a river'>
    </div>
</div>


<style>

.imgContainer {
  position: relative;
  top: 0px;
}

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
  text-decoration: underline;
}

a:active {
  text-decoration: underline;
}
    
  </style>
