<script>
import MicrophoneIcon from "../svelteIcons/MicrophoneIcon.svelte";
import SearchIcon from "../svelteIcons/SearchIcon.svelte";

</script>
<div class="searchbar-container">
    <SearchIcon width="24" height="24"/>
    <input type="text" class="searchbar-input">
    <MicrophoneIcon width="24" height="24" />
</div>

<style>
  .searchbar-container {
    width: auto;
    max-width: 584px;
    background: #202124;
    display: flex;
    align-items: center;
    padding: 0 1rem;
    border: 1px solid #5f6368;
    box-shadow: none;
    border-radius: 24px;
    z-index: 3;
    height: 44px;
    margin: 0 auto;
  }

  .searchbar-input {
    background-color: transparent;
    border: none;
    margin: 0;
    padding: 0 .8rem;
    color: #e8eaed;
    word-wrap: break-word;
    outline: none;
    display: flex;
    flex: 100%;
    height: 34px;
    font-size: 16px;
  }
</style>