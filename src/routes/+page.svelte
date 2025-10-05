<script>
    import Navbar from "$lib/navbar.svelte";
    import { base } from "$app/paths";
</script>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    :global(html,body) {
        margin: 0;
        padding: 0;
    }

    #wrapper {
        background-image: linear-gradient(rgb(6,17,29), rgb(84,19,51));
        min-height: 100vh;
        color: white;
    }

    #view {
        position: relative;
        aspect-ratio: 1/1;
        margin: 0 auto;

        img {
            position: absolute;
            width: 50%;
            height: 50%;
        }
    }

</style>

<div id="wrapper">
    <Navbar />
    <div id="view">

    </div>
</div>
