<script lang="ts">
import AppsIcon from "../svelteIcons/AppsIcon.svelte";
import Link from "../atoms/Link.svelte";
import UserIcon from "../svelteIcons/UserIcon.svelte";

const linkTexts: Array<string> = ["Gmail", "Images"]

</script>
<header>
  <div class="icons-links">
    {#each linkTexts as linkTxt}
      <Link linkClass="white-link" text={linkTxt}/>
    {/each}
    <div class="apps-icon-container">
      <AppsIcon width="24" height="24" />
    </div>
    <a href="https://www.instagram.com/102.tomes/" target="_blank" class="user-icon-container">
      <UserIcon />
    </a>
  </div>
</header>

<style>
  header {
    display: flex;
    justify-content: flex-end;
    width: 100%;
    position: fixed;
    top: 0;
    padding: 1rem;
  }
  .icons-links {
    width: 210px;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }

  .user-icon-container, .apps-icon-container {
    cursor: pointer;
    height: 40px;
    transition: all .3s;
  }

  .user-icon-container {
    padding: 4px;
  }
  .user-icon-container:hover, .apps-icon-container:hover {
    border-radius: 50%;
    background-color: rgba(232,234,237,0.10);
  }

  .apps-icon-container {
    padding: 8px;
  }
</style>