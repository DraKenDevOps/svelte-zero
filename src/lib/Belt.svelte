<script>
  let name = "Owen";
  let belt = "white";

  const changeBelt = () => {
    belt = "blue";
  };

  //   const onInput = (e) => {
  //     belt = e.target.value;
  //   };
</script>

<!-- <input type="text" on:input={onInput} value={belt} /> -->
<input
  type="text"
  bind:value={belt}
  style="padding: 0.6em 1.2em;border-radius: 8px;"
/>
<button on:click={changeBelt}>Change</button>

<h1>{name}</h1>
<h3>Belt:</h3>
<h2>{belt.toUpperCase()}</h2>
<div class="belto" style="background-color: {belt};" />

<style scoped>
  .belto {
    width: 300px;
    height: 100px;
  }
</style>
