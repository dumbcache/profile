<script>
    import Contact from "./components/Contact.svelte";
    import TechStack from "./components/TechStack.svelte";
    import Intro from "./components/Intro.svelte";
    import About from "./components/About.svelte";
</script>

<main>
    <Intro />
    <TechStack />
    <About />
    <Contact />
</main>

<style>
    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
