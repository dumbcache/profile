<script>
    import {
        linkedInIcon,
        emailIcon,
        twitterIcon,
        instagramIcon,
    } from "./Icons.svelte";
</script>

<div id="contact" class="contact-wrapper">
    <h1 class="title">Contact</h1>
    <p class="p1">you can drop a mail to</p>
    <a href="mailto:dumbcache@gmail.com">
        <div class="email">
            {@html emailIcon()}
            dumbcache@gmail.com
        </div>
    </a>
    <p class="p2">get in touch through</p>
    <div class="social">
        <a href="https://twitter.com/yesu4658" target="_blank"
            >{@html twitterIcon()}</a
        >
        <a href="https://www.linkedin.com/in/yesu4658/" target="_blank"
            >{@html linkedInIcon()}</a
        >
        <a href="https://www.instagram.com/yesu4658/" target="_blank"
            >{@html instagramIcon()}</a
        >
    </div>
</div>

<style>
    .contact-wrapper {
        /* border: 1px solid #000; */
        margin-top: 4rem;
        display: flex;
        flex-flow: column;
        align-items: center;
        padding: 1rem;
        margin-bottom: 2rem;
    }
    h1 {
        padding-top: 4rem;
        text-align: center;
    }

    .email {
        display: flex;
        align-items: center;
        border: 1px solid #000;
        width: fit-content;
        padding: 0.5rem;
        border-radius: 1rem;
    }
    .email :global(svg) {
        width: 40px;
        height: auto;
        padding: 0rem 0.2rem;
        margin: 0rem 0.2rem;
    }
    .social :global(svg) {
        width: 40px;
        height: auto;
    }

    .p1 {
        margin: 1rem 0rem;
    }
    .p2 {
        margin: 1rem 0rem;
    }
</style>
