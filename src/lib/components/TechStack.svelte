<script>
    import { Icons } from "./Icons.svelte";
</script>

<section id="skills" class="techstack-wrapper section">
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
    .stack {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-evenly;
    }

    .skill {
        width: 15rem;
        text-align: center;
        padding: 1rem;
    }

    .skill :global(svg) {
        width: 100%;
        height: inherit;
    }
    @media (max-width: 640px) {
        .skill {
            width: 9rem;
        }
    }
</style>
