<script>
    import { Icons } from "./Icons.svelte";
</script>

<div class="footer-wrapper">
    <p>
        Develped by <span>Yesu G</span> <small>(MySelf)</small> using

        <span>
            svelte<sub>{@html Icons.svelte("#444")} </sub>
        </span>
    </p>
</div>

<style>
    .footer-wrapper {
        text-align: center;
        margin-bottom: 4rem;
        color: #888;
    }
    small {
        font-size: xx-small;
    }
    span {
        color: #000;
    }
</style>
