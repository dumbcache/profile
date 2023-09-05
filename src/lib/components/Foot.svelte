<script>
    import { Icons } from "./Icons.svelte";
</script>

<footer class="footer-wrapper section">
    <p>
        Develped by <span>Yesu G</span> <small>(MySelf)</small> using

        <span>
            <a href="https://kit.svelte.dev/">svelte</a><sub
                >{@html Icons.svelte("#444")}
            </sub>
        </span>
    </p>
</footer>

<style>
    .footer-wrapper {
        text-align: center;
        font-size: 1.5rem;
    }
    small {
        font-size: xx-small;
    }
    span {
        color: #f00;
    }
    a:hover {
        color: #00f;
    }
</style>
