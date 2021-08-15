<script lang="ts">
import LanguageText from "./components/LanguageText.svelte";
import SearchBar from "./components/SearchBar.svelte";
import SearchButtons from "./components/SearchButtons.svelte";
import GoogleLogo from "./assets/googlelogo_light_color_272x92dp.png";

</script>

<main>
  <img class="google-logo" src={GoogleLogo} alt="Google">
  <SearchBar />
  <SearchButtons />
  <LanguageText />
</main>

<style>
  :root {
    background-color: #202124;
    font-family: Arial, sans-serif;
    font-size: 14px;
  }

  .google-logo {
    margin-bottom: 2rem;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
</style>
