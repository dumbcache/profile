<script>
    import { Icons } from "./Images.svelte";
</script>

<div>TechStack</div>
{#each Icons as icon}
    <span>{@html icon()}</span>
{/each}
