<div id="about" class="about-wrapper">
    <h1 class="title">MySelf</h1>
    <div class="body">
        <img
            src="https://media-exp1.licdn.com/dms/image/D5603AQGynCfnn7fh3Q/profile-displayphoto-shrink_800_800/0/1648303778377?e=1653523200&v=beta&t=VT6eTL2Swg2vvOxYXVzt76-5EwOjDqY3-792he4jgjc"
            alt="profile pic"
        />
        <p class="info">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus
            commodi necessitatibus repellendus tempore aspernatur dignissimos
            fugiat laudantium quidem quis laborum placeat, accusantium alias
            omnis voluptatum architecto. Praesentium ut officia maiores.
            Similique asperiores error ea doloribus mollitia, odio, natus sed
            dolore modi architecto quam. Possimus eligendi quis, vel aut
            incidunt odio natus molestias nulla ipsum at suscipit id cumque
            dolorum. Laborum dolores,
        </p>
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

    @media (max-width: 640px) {
        .body {
            flex-flow: row wrap;
        }
    }
</style>
