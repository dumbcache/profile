<script>
    import { Icons } from "./Icons.svelte";
</script>

<div id="tech" class="techstack-wrapper">
    <h1 class="title">Skills</h1>
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
</div>

<style>
    .techstack-wrapper {
        margin-top: 4rem;
        /* border: 1px solid #000; */
    }

    .stack {
        display: grid;
        /* border: 1px solid #000; */
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        justify-items: center;
    }

    .skill {
        width: 150px;
        text-align: center;
    }

    .skill :global(svg) {
        width: 100%;
        height: inherit;
    }
    h1 {
        padding-top: 6rem;
        text-align: center;
        margin-bottom: 1rem;
    }
    @media (max-width: 640px) {
        .stack {
            display: initial;
            width: fit-content;
            margin: auto;
        }
        .skill {
            display: inline-block;
            text-align: center;
            width: 100px;
            margin-bottom: 2rem;
        }
    }
</style>
