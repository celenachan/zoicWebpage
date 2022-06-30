<script>
  import { onMount } from "svelte";

  const navItems = [
  { label: "Intro", href: "#"},
//   { label: "Cache options", href: "#"},
//   { label: "Example", href: "#"},
  { label: "DevTool", href: "#"},
  { label: "Contact Info" ,href: "#"}
]
</script>

<nav>
  <div class="navBar">
    <ul class="navbar-list">
      {#each navItems as item}
        <a href={item.href}>{item.label}</a>
      {/each}
    </ul>
  </div>
</nav>

<style>
    nav {
      background-color: rgba(0, 0, 0, 0.8);
      font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
      height: 45px;
      opacity: 80%;
      font-size: 2em;
    }
  
    .navbar-list {
      display: none;
      justify-content: start;
      margin: 0;
      padding: 0 40px;
    }
  
    .navbar-list a {
      color: #fff;
      font-weight: bold;
      text-decoration: underline;
      height: 45px;
      display: flex;
      align-items: center;
      padding: 0 10px;
      font-size: 13px;
      margin: 0 10px;
    }
  
      .navbar-list {
        display: flex;
      }
  
      .navbar-list a {
        display: inline-flex;
        padding: 0;
      }
    
  </style>
