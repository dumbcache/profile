<script>
    import { Icons } from "./Icons.svelte";
</script>

<section id="skills" class="techstack-wrapper">
    <header>
        <h1 class="title">Skills</h1>
    </header>
    <div class="stack">
        {#each Object.entries(Icons) as [name, icon]}
            <div class="skill">
                <div>
                    {@html icon("#444")}
                </div>
                <p>{name}</p>
            </div>
        {/each}
    </div>
</section>

<style>
    .techstack-wrapper {
        margin-top: 4rem;
        /* border: 1px solid #000; */
    }

    .stack {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-evenly;
    }

    .skill {
        width: 150px;
        text-align: center;
        padding: 1rem;
    }

    .skill :global(svg) {
        width: 100%;
        height: inherit;
    }
    .title {
        padding-top: 6rem;
        text-align: center;
        margin-bottom: 2rem;
    }
    @media (max-width: 640px) {
        .skill {
            width: 100px;
        }
    }
</style>
