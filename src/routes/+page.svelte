<script>
    import Navbar from "$lib/navbar.svelte";
    import { base } from "$app/paths";
</script>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

    :global(html,body) {
        margin: 0;
        padding: 0;
        background-color: black;

        font-family: Montserrat;
    }

    .navbar {
        position: absolute;
        z-index: 1000;
        top: 0;
        right: 0;
        left: 0;
        height: 70px;
        overflow: hidden;
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

    #content {
        background-color: rgb(41,41,42);
        padding: 20px;
    }

</style>
<Navbar class="navbar"/>
<div id="wrapper">
    <div id="view">
        <img src="logo/logo-dark.png" style="width: 20%; height: auto; left: 40%; right: 40%; top: 110px;" alt="Logo" />
        <img src="views/main/4.png" alt="Cloud Layer" />
        <img src="views/main/5.png" alt="Cloud Layer" />
        <img src="views/main/6.png" alt="Cloud Layer" />
        <img src="views/main/7.png" alt="Cloud Layer" />
    </div>
    <div id="content">
        <br><br>
        <h1 style="font-weight: 800">What is Étoile?</h1>
        <h3>Qu'est-ce que l'Étoile?</h3>
    </div>
</div>
