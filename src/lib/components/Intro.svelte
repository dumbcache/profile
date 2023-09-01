<script>
    import { locationIcon1 } from "./Icons.svelte";
</script>

<div id="intro" class="intro-wrapper">
    <div class="name">Yesu G,</div>
    <div class="profession">
        <div>Web</div>
        Developer
    </div>
    <div class="location">
        {@html locationIcon1()} Vijayawada, India
    </div>
    <p class="intro">
        `` I'm a computer science graduate aspiring to become web and mobile
        application developer ``
    </p>
</div>

<style>
    .intro-wrapper {
        /* border: 1px solid #000; */
        /* margin-top: 1rem; */
        padding: 1rem;
    }
    .name {
        font-size: 4vw;
        font-weight: 700;
        font-family: poiret one;
        padding-top: 6rem;
        user-select: none;
        margin-bottom: 1rem;
    }
    .profession {
        font-size: 10vw;
        font-weight: 900;
        user-select: none;
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

    @media (max-width: 640px) {
        .name {
            font-size: 6vmax;
        }
        .profession {
            font-size: 7vmax;
        }
    }
</style>
