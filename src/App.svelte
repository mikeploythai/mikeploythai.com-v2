<script lang="ts">
  /* export let name: string; */
  import Navbar from "../components/UI/Navbar.svelte";
  import Hero from "../components/index/Hero.svelte";
</script>

<main>
  <Navbar />
  <Hero />
</main>

<style lang="scss">
  main {
    position: relative;
    background-color: var(--baby-blue);
    min-height: 100vh;
  }
</style>
