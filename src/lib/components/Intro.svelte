<script>
    import { locationIcon1 } from "./Icons.svelte";
    import experienceIcon from "$lib/assets/experience.png";
</script>

<section id="intro" class="intro-wrapper section">
    <header>
        <h1 class="name">Yesu G,</h1>
        <h2 class="profession">
            <div>Web</div>
            Developer
        </h2>
    </header>
    <div class="content">
        <p class="location">
            {@html locationIcon1()} Vijayawada, India
        </p>
        <!-- <p>
            <img src={experienceIcon} alt="" width="30" height="30" />
            2+ years
        </p> -->
        <p class="intro">
            ``` I'm a computer science graduate aspiring to become web and
            mobile application developer ```
        </p>
    </div>
</section>

<style>
    .name {
        font-size: 4vw;
        font-weight: 700;
        font-family: poiret one;
        margin-bottom: 1rem;
        padding-bottom: 0;
        text-align: start;
    }
    .profession {
        font-size: 10vw;
        font-weight: 900;
        font-family: poppins, sans-serif;
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
        .section {
            padding-top: 10rem;
        }
        .profession {
            font-size: 7vmax;
        }
    }
</style>
