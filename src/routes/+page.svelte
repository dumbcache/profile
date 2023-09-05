<script>
    import "./app.css";
    import Header from "$lib/components/Header.svelte";
    import Intro from "$lib/components/Intro.svelte";
    import TechStack from "$lib/components/TechStack.svelte";
    import Projects from "$lib/components/Projects.svelte";
    import Myself from "$lib/components/Myself.svelte";
    import Contact from "$lib/components/Contact.svelte";
    import Foot from "$lib/components/Foot.svelte";
</script>

<main>
    <Header />
    <Intro />
    <TechStack />
    <Projects />
    <Myself />
    <Contact />
    <Foot />
</main>

<style>
    @media (max-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
