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

    #wrapper {
        background-image: linear-gradient(rgb(6,17,29), rgb(84,19,51));
        min-height: 100vh;
        color: white;
    }

    #view {
        position: relative;
        aspect-ratio: 1/0.56;
        margin: 0 auto;
        overflow: hidden;

        img {
            position: absolute;
            width: 100%;
            height: 100%;
        }

        #logo-view {
            width: 20%; 
            height: auto; 
            left: 40%; 
            right: 40%; 
            top: 150px;
        }
    }

    @media screen and (max-width: 900px) {
        #view #logo-view {
            top: 100px;
        }
    }


    #content {
        background-color: rgb(41,41,42);
        padding: 20px;

        text-align: center;
    }

    @keyframes cloud-move {
        0% {transform: translateY(0px);}
        50% {transform: translateY(20px);}
        100% {transform: translateY(0px);}
    }

    #cloud1{
        animation: cloud-move 5s ease-in-out infinite;
    }
    #cloud2{
        animation: cloud-move 5s ease-in-out infinite;
        animation-delay: 0.5s;
    }
    #cloud3{
        animation: cloud-move 5s ease-in-out infinite;
        animation-delay: 1.2s;
    }

</style>
<Navbar/>
<div id="wrapper">
    <div id="view">
        <img src="logo/logo-dark.png" id="logo-view" alt="Logo" translate = "no"/>
        <img src="views/main/4.png" alt="Cloud Layer" id="cloud1"/>
        <img src="views/main/5.png" alt="Cloud Layer" id="cloud2"/>
        <img src="views/main/6.png" alt="Cloud Layer" id = "cloud3"/>
        <img src="views/main/7.png" alt="Cloud Layer" />
    </div>
    <div id="content">
        <br><br>
        <h1 style="font-weight: 800">What is Étoile?</h1>
        <h3>Qu'est-ce que l'Étoile?</h3>
    </div>
</div>
