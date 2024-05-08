<script>
    import {
        linkedInIcon,
        emailIcon,
        twitterIcon,
        instagramIcon,
    } from "./Icons.svelte";
</script>

<section id="contact" class="contact-wrapper section">
    <header class="header">
        <h1 class="title">Contact</h1>
    </header>

    <div class="content">
        <p class="p1">Drop me a mail here 👇</p>
        <a href="mailto:dumbcache@gmail.com">
            <div class="email">
                {@html emailIcon()}
                dumbcache@gmail.com
            </div>
        </a>
        <p class="p2">get in touch through</p>
        <section class="social">
            <a href="https://twitter.com/yesu4658">{@html twitterIcon()}</a>
            <a href="https://www.linkedin.com/in/dumbcache/"
                >{@html linkedInIcon()}</a
            >
            <a href="https://www.instagram.com/yesu4658/"
                >{@html instagramIcon()}</a
            >
        </section>
    </div>
</section>

<style>
    .email {
        display: flex;
        align-items: center;
        border: 1px solid #f00;
        width: fit-content;
        padding: 0.5rem;
        border-radius: 1rem;
    }
    .email :global(svg) {
        width: 4rem;
        height: auto;
        padding: 0rem 0.2rem;
        margin: 0rem 0.2rem;
    }
    .social :global(svg) {
        width: 4rem;
        height: auto;
    }
    .content {
        display: flex;
        flex-flow: column;
        align-items: center;
    }

    .p1 {
        margin: 1rem 0rem;
    }
    .p2 {
        margin: 1rem 0rem;
    }
    .content {
        text-align: center;
    }

    a {
        width: fit-content;
    }
    @media (max-width: 600px) {
        .social :global(svg) {
            width: 3rem;
            height: auto;
        }
    }
</style>
