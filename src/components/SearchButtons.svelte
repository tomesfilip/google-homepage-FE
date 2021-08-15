<script>
import SearchButton from "../atoms/SearchButton.svelte";
</script>

<div class="search-buttons-container">
  <center>
    <SearchButton inputVal="Google Search" inputName="btnK" />
    <SearchButton inputVal="I'm Feeling Lucky" inputName="btnI" />
  </center>
</div>

<style>
  .search-buttons-container {
    height: 70px;
    padding-top: 18px;
    margin-bottom: 1.2rem;
  }

  center {
    text-align: center;
  }
</style>