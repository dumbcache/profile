<script>
    import {
        linkedInIcon,
        emailIcon,
        twitterIcon,
        instagramIcon,
    } from "./Images.svelte";
</script>

<div class="contact-wrapper">
    <h1 class="title">Contact</h1>
    <p>you can drop a mail here</p>
    <div class="email">
        {@html emailIcon()}
        <a href="mailto:dumbcache@gmail.com"> dumbcache@gmail.com </a>
    </div>
    <p>you can contact me on any of these social platforms</p>
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
        border: 1px solid #000;
        margin-top: 4rem;
    }
    h1 {
        text-align: center;
    }
    a,
    a:link,
    a:visited,
    a:active {
        text-decoration: none;
        color: inherit;
    }
    .email {
        display: flex;
        align-items: center;
        border: 1px solid #000;
        width: fit-content;
        padding: 0.5rem;
    }
    .email :global(svg) {
        width: 40px;
        height: auto;
    }
    .social :global(svg) {
        width: 40px;
        height: auto;
    }
</style>
