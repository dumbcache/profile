<script>
    import Contact from "./components/Contact.svelte";
    import TechStack from "./components/TechStack.svelte";
    import Intro from "./components/Intro.svelte";
    import About from "./components/About.svelte";
    import Header from "./components/Header.svelte";
</script>

<main>
    <Header />
    <Intro />
    <TechStack />
    <About />
    <Contact />
</main>

<style>
    @media (max-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
