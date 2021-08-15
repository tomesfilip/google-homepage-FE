<script lang="ts">
  export let text: string
  export let linkTo: string = "./"
  export let linkClass: string
  export let blank: boolean = false
</script>

<a class={linkClass} href={linkTo} target={blank ? "_blank" : "_self"}>{text}</a>

<style>
  .blue-link, .grey-link, .white-link {
    text-decoration: none;
  }

  .blue-link:hover, .grey-link:hover, .white-link:hover {
    text-decoration: underline;
  }
  .blue-link {
    color: #8ab4f8;
  }
  .white-link {
    color: white;
    line-height: 24px;
    font-size: 13px;
  }

  .grey-link {
    color: #999da2;
    display: block;
    padding: 15px;
    white-space: nowrap;
  }

</style>