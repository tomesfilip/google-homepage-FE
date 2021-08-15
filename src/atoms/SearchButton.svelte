<script lang="ts">
  export let inputVal: string
  export let inputName: string
</script>

<input value={inputVal} aria-label={inputVal} name={inputName} type="submit" >

<style>
  input {
    background-color: #303134;
    border: 1px solid #303134;
    border-radius: 4px;
    color: #e8eaed;
    font-family: arial,sans-serif;
    font-size: 14px;
    margin: 11px 4px;
    padding: 0 16px;
    line-height: 27px;
    height: 36px;
    min-width: 54px;
    text-align: center;
    cursor: pointer;
    user-select: none;
    transition: all .3s;
  }

  input:hover {
    box-shadow: 0 1px 3px rgba(23,23,23,0.24);
    background-color: #303134;
    border: 1px solid #5f6368;
    color: #e8eaed;
  }

  input:focus {
    border: 1px solid #5f6368;
    outline: none;
  }
</style>