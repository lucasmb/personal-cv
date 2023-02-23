<script>
  let count = 0;
  const increment = () => {
    count += 1;
  };
</script>

<h1 class="text-3xl font-bold underline">Hello world!</h1>
<button on:click={increment}>
  count is {count}
</button>
