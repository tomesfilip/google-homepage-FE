<script lang="ts">
import Link from "../atoms/Link.svelte";

const linksLeft: Array<Object> = [
  {
    txt: "About",
    dst: "https://about.google/?utm_source=google-CZ&utm_medium=referral&utm_campaign=hp-footer&fg=1",
  },
  {
    txt: "Advertising",
    dst: "https://www.google.com/intl/en_cz/ads/?subid=ww-ww-et-g-awa-a-g_hpafoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpafooter&fg=1",
  },
  {
    txt: "Business",
    dst: "https://www.google.com/services/?subid=ww-ww-et-g-awa-a-g_hpbfoot1_1!o2&utm_source=google.com&utm_medium=referral&utm_campaign=google_hpbfooter&fg=1",
  },
  {
    txt: "How Search works",
    dst: "https://google.com/search/howsearchworks/?fg=1",
  }
]

const linksRight: Array<Object> = [
  {
    txt: "Privacy",
    dst: "https://policies.google.com/privacy?hl=en-CZ&fg=1",
  },
  {
    txt: "Terms",
    dst: "https://policies.google.com/terms?hl=en-CZ&fg=1",
  },
  {
    txt: "Settings",
    dst: "http://gph.is/1idcey1",
  }
]
</script>

<footer>
  <div class="left-side">
    {#each linksLeft as link}
      <Link linkClass="grey-link" text={link.txt} linkTo={link.dst} />
    {/each}
  </div>
  <div class="right-side">
    {#each linksRight as link}
      <Link linkClass="grey-link" text={link.txt} linkTo={link.dst} />
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