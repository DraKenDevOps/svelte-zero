<script>
  let count = 0;
  const increment = () => {
    count += 1;
  };
</script>

<h1>Ninja Level: {count}</h1>

<button on:click={increment}> COUNT </button>

<style scoped>
  button {
    color: #ffffff;
    background-color: #1b75ba;
  }
</style>
