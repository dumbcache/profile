<script>
    import { locationIcon1, locationIcon2 } from "./components/Images.svelte";

    import TechStack from "./components/TechStack.svelte";
</script>

<main>
    <p>profile</p>
    <img
        src="https://avatars.githubusercontent.com/u/50919263?v=4"
        alt="profile pic"
        width="100"
        height="100"
    />
    <div>
        {@html locationIcon1()}
    </div>

    <TechStack />
</main>

<style>
    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
