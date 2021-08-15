<script lang="ts">
  export let text: string
  export let linkTo: string = "./"
  export let linkClass: string
  export let blank: boolean = false
</script>

<a class={linkClass} href={linkTo} target={blank ? "_blank" : "_self"}>{text}</a>

<style>
  .blue-link {
    color: #8ab4f8;
    text-decoration: none;
  }
  .white-link {
    color: white;
    text-decoration: none;
  }

  .grey-link {
    color: #999da2;
    display: block;
    padding: 15px;
    white-space: nowrap;
    text-decoration: none;
  }

</style>