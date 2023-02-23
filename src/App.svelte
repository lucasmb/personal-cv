<script>
  import svelteLogo from "./assets/svelte.svg";
  import Counter from "./lib/Counter.svelte";
  import data from "./data.json";
</script>

<main class="container md:container md:mx-auto px-1">
  <div class="grid py-2 gap-4 grid-cols-3 grid-rows-3 ">
    <div class=" bg-red-100">
      <div
        class="py-1"
        style="background: linear-gradient(90deg, black 50%, transparent 0%);"
      >
        <img
          class="mx-10 h-300 w-300 rounded-full ring-4 ring-black"
          src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
          alt=""
        />
      </div>
    </div>
    <div class="justify-self-start col-span-2">
      <div class="text-3xl font-bold ">{data.header}</div>
      <div>subtitle</div>
    </div>
    <div class="content-center">
      Contact
      <ul>
        <li>
          {data.contact.phone}
        </li>
        <li />
      </ul>
    </div>
    <div>04</div>
    <div>05</div>
    <div>Skillz</div>
  </div>
  <div class="card">
    <Counter />
  </div>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
  }
</style>
