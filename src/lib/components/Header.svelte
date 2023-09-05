<header class="header">
    <nav class="navigation">
        <a href="#intro">
            <div>Home</div>
        </a>
        <a href="#skills">
            <div>Skills</div>
        </a>
        <a href="#projects">
            <div>Projects</div>
        </a>

        <a href="#myself">
            <div>MySef</div>
        </a>
        <a href="#contact">
            <div>Contact</div>
        </a>
    </nav>
</header>

<style>
    .header {
        position: fixed;
        top: 0px;
        left: 0px;
        width: 100%;
        background-color: #fff;
        z-index: 1;
    }
    .navigation {
        display: flex;
        justify-content: space-around;
        padding: 2rem 0rem;
    }

    @media (max-width: 600px) {
        .header {
            font-size: 1.3rem;
        }
    }
</style>
