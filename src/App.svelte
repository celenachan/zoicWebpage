<script>
  import NavBar from './lib/Navbar.svelte';
  import MainLanding from './lib/MainLanding.svelte';
  import Intro from './lib/Intro.svelte';
  import CacheCustomization from './lib/CacheCustomization.svelte';
  import CodeExample from './lib/CodeExample.svelte';
  import DevTools from './lib/DevTools.svelte';
  import ContactInfo from './lib/ContactInfo.svelte';
</script>

<main>

  <div class="websiteContainer">
    <div class="navBar">
      <NavBar />
    </div>
    <div class="mainLanding">
      <MainLanding />
    </div>
    <div class="intro">
      <Intro />
    </div>
    <div class="CacheCustomization">
      <CacheCustomization />
    </div>
    <div class="codeExample">
      <CodeExample />
    </div>
    <div class="devTools">
      <DevTools />
    </div>
    <div class="contactInfo">
      <ContactInfo />
    </div>
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

  .websiteContainer {
    margin: -10px;
    background-color: black;
  }

</style>
