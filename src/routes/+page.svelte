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
        aspect-ratio: 1/0.56;
        margin: 0 auto;

        img {
            position: absolute;
            width: 100%;
            height: 100%;
        }
    }

</style>

<div id="wrapper">
    <Navbar />
    <div id="view">
        <img src="logo/logo-dark.png" style="width: 20%; height: auto; left: 40%; right: 40%; top: 110px;" alt="Halo" />
        <img src="views/main/2.png" alt="Halo" />
        <img src="views/main/3.png" alt="Halo" />
        <img src="views/main/4.png" alt="Halo" />
        <img src="views/main/5.png" alt="Halo" />
        <img src="views/main/6.png" alt="Halo" />
        <img src="views/main/7.png" alt="Halo" />
    </div>
</div>
