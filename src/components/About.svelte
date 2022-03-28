<script>
    import { Icons } from "./Icons.svelte";
</script>

<div id="about" class="about-wrapper">
    <h1 class="title">MySelf</h1>
    <div class="body">
        <div class="head">
            <img
                src="https://media-exp1.licdn.com/dms/image/D5603AQGynCfnn7fh3Q/profile-displayphoto-shrink_800_800/0/1648303778377?e=1653523200&v=beta&t=VT6eTL2Swg2vvOxYXVzt76-5EwOjDqY3-792he4jgjc"
                alt="profile pic"
            />
            <!-- <p>Yesu Gudi</p>
            <p>2years experience</p> -->
            <!-- <p>`` coding is fun 😁 ``</p> -->
        </div>

        <div class="info">
            <p>Hey there👋, Yesu here</p>
            <p>
                I am Computer Science B.Tech graduate🧑‍🎓 from Vijayawada,
                India. Currently working as software associate <small>
                    (still web deveolper to core).
                </small>
            </p>
            <p>
                I got interest in Web Development during the final year of my
                B.Tech. I am impressed and ashtonished by the web and how it
                works and hooked onto a single thought that " I should definetly
                choose this as my career".
            </p>
            <p>
                From then, I started learning the core of the web fundamentals.
                I work on both UI and Backend API's.
            </p>
            <p>
                View my projects <a
                    href="https://github.com/yesu4658"
                    target="_blank"
                >
                    here<sub>
                        {@html Icons.github()}
                    </sub>
                </a>
            </p>
        </div>
    </div>
</div>

<style>
    .about-wrapper {
        /* border: 1px solid #000; */
        margin-top: 4rem;
    }

    .title {
        padding-top: 6rem;
        text-align: center;
    }
    img {
        width: 300px;
        height: 300px;
        border-radius: 50%;
    }
    .body {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .body > * {
        padding: 1rem;
    }

    small {
        color: #444;
    }
    p {
        margin-bottom: 0.5rem;
    }
    sub :global(svg) {
        width: 40px;
        height: auto;
    }
    @media (max-width: 800px) {
        .body {
            flex-flow: row wrap;
        }
    }
</style>
