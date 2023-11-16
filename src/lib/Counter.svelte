<svelte:options
  customElement={{
    tag: "my-counter",
  }}
/>

<script>
  let count = 0;
  const increment = () => {
    count += 2;
  };
</script>

<div class="container">
  <button on:click={increment}>
    count is {count}
  </button>
</div>

<style lang="scss">
  .container {
    margin: 30px;
    button {
      font-size: 20px;
      color: rgb(0, 255, 13);
    }
  }
</style>
