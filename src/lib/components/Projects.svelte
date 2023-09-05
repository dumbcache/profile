<script>
    import linkIcon from "$lib/assets/link.svg?raw";
</script>

<section id="projects" class="projects-wrapper section">
    <header>
        <h1 class="title">Projects</h1>
    </header>

    <div class="content">
        <article class="article">
            <h3>
                Pocket Drive

                <sub class="icon">
                    <a href="https://pocketdrive.vercel.app">{@html linkIcon}</a
                    ></sub
                >
            </h3>

            <p>A google drive based image & bookmark application</p>
            <section class="features">
                <h5>features</h5>
                <ul>
                    <li>Add URL's to images for easy bookmarking</li>
                    <li>Favourite your images for easy filter</li>
                    <li>Edit mode to easily update, move and delete</li>
                    <li>Upload images by dropping</li>
                    <li>Easy folder searching</li>
                </ul>
            </section>
        </article>
        <article class="article">
            <h3>
                Pocket Drive Chrome Extension

                <sub class="icon">
                    <a
                        href="https://github.com/dumbcache/pocketdrive-chrome-extension"
                        >{@html linkIcon}</a
                    ></sub
                >
            </h3>
            <p>A google drive based image & bookmark application</p>
            <section class="features">
                <h5>features</h5>
                <ul>
                    <li>Easy to use</li>
                    <li>Save by right click on image in website</li>
                    <li>Search and create folders easily</li>
                </ul>
            </section>
        </article>
    </div>
</section>

<style>
    .section {
        line-height: 1.5;
    }
    h3 {
        color: #f00;
        filter: invert(0.1);
        padding-bottom: 0.5rem;
    }

    .content {
        display: flex;
        gap: 2rem;
        justify-content: space-evenly;
    }
    .article {
        padding: 1rem;
    }

    .icon {
        width: 2rem;
    }
    .icon :global(svg) {
        width: 2rem;
    }
    .icon:hover :global(svg) {
        fill: red;
    }
    .features {
        padding-top: 1rem;
    }
    h5 {
        text-decoration: underline;
    }

    @media (max-width: 600px) {
        .content {
            flex-flow: column;
            align-items: center;
        }
    }
</style>
