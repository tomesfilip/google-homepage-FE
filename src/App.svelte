<script lang="ts">
import LanguageText from "./components/LanguageText.svelte";
import SearchBar from "./components/SearchBar.svelte";
import SearchButtons from "./components/SearchButtons.svelte";
import GoogleLogo from "./assets/googlelogo_light_color_272x92dp.png";
import Footer from "./components/Footer.svelte";
import TopPanel from "./components/TopPanel.svelte";
</script>

<TopPanel />
<main>
  <img class="google-logo" src={GoogleLogo} alt="Google">
  <SearchBar />
  <SearchButtons />
  <LanguageText />
</main>
<Footer />

<style>
  :root {
    background-color: #202124;
    font-family: Arial, sans-serif;
    font-size: 14px;    
  }
  main {
    width: 100%;
    text-align: center;
    padding: 1rem;
    margin-bottom: 14%;
  }

  .google-logo {
    margin-bottom: 1rem;
  }
</style>
