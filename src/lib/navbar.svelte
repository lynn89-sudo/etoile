<script>
    import { base } from "$app/paths";
</script>
<style>
     @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
     @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300..700&display=swap');
    * {
        font-family: Montserrat;
        color: white;
        text-align: center;
    }

    .material-symbols-outlined {
        vertical-align: -6px;
        margin-left: 4px;
    }

    #container {
        position: fixed;
        z-index: 1000;
        top: 0;
        right: 0;
        left: 0;
        height: 70px;
        background-color: rgba(34, 34, 34, 0.884);
        overflow: hidden;

        user-select: none;
        -webkit-user-select: none;
        -webkit-user-drag: none;
        -moz-user-select: none;

        cursor: pointer;

        #flightInfo {
            position: absolute;
            right: 30%;
            left: 30%;
            width: 40%;
            top: 8px;

            transition: top 1.5s ease-in-out;
        }

        td.head {
            font-family: Space Grotesk, Montserrat;
        }
        td {
            font-weight: 800;
        }
    }

    @media screen and (max-width: 950px) {
        #container {
            #flightInfo {
                right: 15%;
                left: 15%;
                width: 70%;
            }
        }
    }
     @media screen and (max-width: 700px) {
        #container {
            #flightInfo {
                right: 5%;
                left: 5%;
                width: 90%;
            }
        }
    }
    #container:hover {
        #flightInfo {
            top: -80px;
        }
    }
</style>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200&icon_names=airlines,airplane_ticket,flight,flight_land,flight_takeoff,kid_star,location_chip,plane_contrails" />

<div id="container">
    <table id="flightInfo">
        <tbody>
            <tr>
                <td class="head">
                    | FLIGHT |
                </td>
                <td class="head">
                    | DESTINATION |
                </td>
                 <td class="head">
                    | STATUS |
                </td>
            </tr>
            <tr>
                <td>HC 001<span translate = "no" class="material-symbols-outlined">airlines</span></td>
                <td translate = "no">L'ÉTOILE<span  translate = "no" class="material-symbols-outlined">location_chip</span></td>
                <td style="color: lightgreen;">CHECK-IN<span  translate = "no" class="material-symbols-outlined">airplane_ticket</span></td>
            </tr>
        </tbody>
    </table>
</div>