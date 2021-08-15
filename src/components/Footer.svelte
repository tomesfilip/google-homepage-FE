<script lang="ts">
import Link from "../atoms/Link.svelte";

const linkTextsLeft: Array<string> = ["About", "Advertising", "Business", "How Search works"]
const linkTextsRight: Array<string> = ["Privacy", "Terms", "Settings"]

</script>
<footer>
  <div class="left-side">
    {#each linkTextsLeft as linkTxt}
      <Link linkClass="grey-link" text={linkTxt} />
    {/each}
  </div>
  <div class="right-side">
    {#each linkTextsRight as linkTxt}
      <Link linkClass="grey-link" text={linkTxt} />
    {/each}
  </div>
</footer>

<style>
  footer {
    position: fixed;
    bottom: 0;
    display: flex;
    width: 100%;
    justify-content: space-between;
    padding: 0 1rem;
    background-color: #171717;
  }

  .left-side, .right-side {
    display: flex;
    flex-wrap: wrap;
  }
</style>