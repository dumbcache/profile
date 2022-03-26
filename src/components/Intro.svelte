<script>
    import { locationIcon1 } from "./Images.svelte";
</script>

<div class="intro-wrapper">
    <div class="name">Yesu G,</div>
    <div class="profession">
        <div>Web</div>
        Developer
    </div>
    <div class="location">
        {@html locationIcon1()} Vijayawada, India
    </div>
    <p class="intro">
        `` I'm a computer science graduate.I started my career aiming to become
        web and mobile application developer. I feel coding very fun. ``
    </p>
</div>

<style>
    .intro-wrapper {
        border: 1px solid #000;
        margin-top: 1rem;
    }
    .name {
        font-size: 4vw;
        font-weight: 700;
        font-family: poiret one;
    }
    .profession {
        font-size: 10vw;
        font-weight: 900;
    }
    .name,
    .profession {
        line-height: 1;
    }
    .intro {
        margin-top: 3rem;
    }
    .location {
        display: flex;
        margin: 1rem 0rem;
        align-items: center;
    }
</style>
