<script>
  import NavBar from './lib/Navbar.svelte';
  import CacheCustomization from './lib/CacheCustomization.svelte';
  import CodeExample from './lib/CodeExample.svelte';
  import DevTools from './lib/DevTools.svelte';
  import ContactInfo from './lib/ContactInfo.svelte';

  const navItems = [
  { label: "Intro", href: "#introLink"},
//   { label: "Cache options", href: "#"},
//   { label: "Example", href: "#"},
  { label: "Dev Tool", href: "#devToolLink"},
  { label: "Contact Info" ,href: "#contactLink"}
]
</script>

<main>

  <div class="websiteContainer">
    <div class="navBar">
      <NavBar {navItems}/>
    </div>
    <a id="introLink">
    <div class="codeExample">
      <CodeExample />
    </div>
    <div class="CacheCustomization">
      <CacheCustomization />
    </div>
    </a>
    <a id="devToolLink">
    <div class="devTools">
      <DevTools />
    </div>
    </a> 
    <a id="contactLink">
    <div class="contactInfo">
      <ContactInfo />
    </div>
  </a>
  </div>

  <!-- <img src={logo} alt="Svelte Logo" />
  <h1>Hello world!</h1>

  <Counter />

  <p>
    Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte
    apps. 
  </p>

  <p>
    Check out <a href="https://github.com/sveltejs/kit#readme">SvelteKit</a> for
    the officially supported framework, also powered by Vite!
  </p> -->
</main>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  body {
    margin: 0 0 0 0;

  }

  

  .websiteContainer {
    margin: -10px;
    /* background-color: black; */
    background-color: black;
    background-image: linear-gradient(#2E485D, 20%, #EE892F,  #E76020, #E0BB76, #6E896A);
    margin: 0 0 0 0;
    margin-top: -10px;
    margin-left: -10px;
    margin-right: -10px;
    display: flex;
    flex-direction: column;
  }

  
  

</style>
