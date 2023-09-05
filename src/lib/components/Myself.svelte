<script>
    import { githubIcon } from "./Icons.svelte";
    import { onMount } from "svelte";
    let profilePic;

    onMount(async () => {
        let req = await fetch("https://api.github.com/users/dumbcache");
        let data = await req.json();
        profilePic = data["avatar_url"];
    });
</script>

<section id="myself" class="myself-wrapper section">
    <header class="header">
        <h1 class="title">MySelf</h1>
    </header>
    <div class="content">
        {#if profilePic}
            <img src={profilePic} alt="profile pic" />
        {/if}

        <aside class="tail">
            <p>Hey there 👋 ,</p>
            <p>
                I am Computer Science B.Tech graduate🧑‍🎓 from Vijayawada, India.
                I've got work experience of 2+ years.
            </p>
            <br />
            <p>
                I got interest in Web Development during the final year of my
                B.Tech. I am impressed and ashtonished by the web and how it
                works and hooked onto a single thought that "I should definetly
                choose this as my career".
            </p>
            <br />
            <p>
                From then, I started learning Web. I work on both UI and Backend
                API's.
            </p>
            <p>
                View my projects <a href="https://github.com/dumbcache">
                    here<sub>
                        {@html githubIcon()}
                    </sub>
                </a>
            </p>
        </aside>
    </div>
</section>

<style>
    .section {
        line-height: 1.5;
    }
    img {
        width: 300px;
        border-radius: 50%;
    }

    .content {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 5rem;
    }
    .content > * {
        padding: 1rem;
    }

    sub :global(svg) {
        width: 40px;
        height: auto;
    }
    a {
        color: blue;
    }
    @media (max-width: 800px) {
        .content {
            flex-flow: row wrap;
            gap: 2rem;
        }

        img {
            max-width: 70%;
        }
    }
</style>
