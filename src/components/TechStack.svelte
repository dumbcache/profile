<script>
    import { Icons } from "./Images.svelte";
</script>

<div class="techstack-wrapper">
    <h1 class="title">Tech Knowledge</h1>
    <div class="stack">
        {#each Icons as icon}
            <span>{@html icon()}</span>
        {/each}
    </div>
</div>

<style>
    .techstack-wrapper {
        margin-top: 4rem;
        border: 1px solid #000;
    }
    .title {
        text-align: center;
        /* font-size: 4vw; */
        /* font-weight: 900; */
    }
    .stack {
        /* background-color: #fff; */
        border: 1px solid #000;
        width: fit-content;
    }
    .stack :global(svg) {
        width: 60px;
        height: auto;
    }
</style>
