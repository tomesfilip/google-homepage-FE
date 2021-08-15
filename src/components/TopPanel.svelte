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
    <AppsIcon width="24" height="24" />
    <UserIcon />
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
    width: 200px;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
</style>