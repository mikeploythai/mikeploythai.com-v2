<script lang="ts">
	import Navbar from "../components/ui/Navbar.svelte";
	import Hero from "../components/index/Hero.svelte";
	import Projects from "../components/index/Projects.svelte";
	import About from "../components/index/About.svelte";
	import Footer from "../components/ui/Footer.svelte";
</script>

<main>
	<Navbar />
	<Hero />
	<Projects />
	<About />
	<Footer />
</main>

<style lang="scss">
	main {
		position: relative;
		display: flex;
		flex-direction: column;
		gap: 128px;
		background-color: var(--baby-blue);
		min-height: 100vh;
	}
</style>
