<script lang="ts">
import Link from "../atoms/Link.svelte";
</script>

<div class="lang-text">
  Google offered in: <Link linkClass="blue-link" linkTo="https://en.wikipedia.org/wiki/Slovakia" blank={true} text="Slovak" />
</div>

<style>
  .lang-text {
    display: inline-block;
    line-height: 28px;
    color: #bdc1c6;
    font-size: small;
  }
</style>