<!DOCTYPE html>
<html lang="es">

<head>
    <title>Gamerland</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #1c1c1c;
            color: #f5f5f5;
            background-image: url('https://scontent.fgye7-1.fna.fbcdn.net/v/t39.30808-6/401848894_972391327738305_5082667008647218459_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=cc71e4&_nc_ohc=zr6G4BULKFsQ7kNvgEFJtLZ&_nc_zt=23&_nc_ht=scontent.fgye7-1.fna&_nc_gid=A-QKKiuJJccfvUfvUSAwNjI&oh=00_AYCg1K_yQAwjSIg5oZssxQzO5BMAVO-fUxnz3MOLcUIBgw&oe=676FE7C0');
            background-size: cover;
            background-attachment: fixed;
        }

        header {
            background-color: rgba(30, 30, 47, 0.8);
            padding: 20px;
            text-align: center;
        }

        header h1,
        header h2,
        header p {
            animation: fadeInDown 1.5s ease-in-out;
        }

        .container {
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            margin: 20px;
            animation: fadeInUp 1.5s ease-in-out;
        }

        .info h2 {
            color: #ff9800;
            animation: fadeInLeft 1.5s ease-in-out;
        }

        .promo {
            background-color: rgba(46, 46, 64, 0.8);
            padding: 20px;
            border-radius: 8px;
            animation: pulse 2s infinite;
        }

        .promo h3 {
            color: #ff9800;
            margin-bottom: 10px;
        }

        .contacto {
            margin-top: 20px;
        }

        .contacto a {
            color: #ff9800;
            text-decoration: none;
            font-weight: bold;
            animation: shakeX 1.5s infinite;
        }

        .competencia {
            background-color: rgba(46, 46, 64, 0.8);
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
            animation: bounceIn 1.5s ease-in-out;
        }

        .button {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background-color: #ff9800;
            color: #121212;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            animation: heartBeat 2s infinite;
            transition: transform 0.3s ease-in-out;
        }

        .button:hover {
            transform: scale(1.1);
        }

        footer {
            text-align: center;
            padding: 10px;
            background-color: rgba(30, 30, 47, 0.8);
            color: #888;
            animation: fadeInUp 1.5s ease-in-out;
        }

        .gaming-image {
            text-align: center;
            margin: 20px 0;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
        }

        .gaming-image img {
            max-width: 45%;
            height: auto;
            border-radius: 10px;
            border: 2px solid rgba(255, 255, 255, 0.6);
            animation: zoomIn 1.5s ease-in-out;
            transition: transform 0.3s ease-in-out;
        }

        .gaming-image img:hover {
            transform: scale(1.1);
            box-shadow: 0 0 15px rgba(255, 152, 0, 0.8);
        }

        .gaming-image .circle-image {
            max-width: 15%;
            border-radius: 50%;
            border: 3px solid rgba(255, 255, 255, 0.8);
            animation: rotateIn 1.5s ease-in-out;
        }
        .modal {
            display: none;
            /* Oculto por defecto */
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            justify-content: center;
            align-items: center;
            animation: fadeIn 1.5s;
        }

        .modal-content {
            background-color: #333;
            color: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            animation: zoomIn 1.5s ease-in-out;
        }

        .close {
            color: #fff;
            font-size: 30px;
            font-weight: bold;
            position: absolute;
            top: 10px;
            right: 20px;
            cursor: pointer;
        }
    </style>
</head>

<body>
    <header>
        <h1>Gamerland</h1>
        <h2>Machala</h2>
        <p>La mejor experiencia gaming en El Oro</p>
    </header>

    <!-- Modal -->
    <div id="myModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2>¡Bienvenido a Gamerland!</h2>
            <p>Estamos emocionados de que estés aquí. ¡Disfruta de la mejor experiencia gaming!</p>
        </div>
    </div>

    <div class="container">
        <div class="info">
            <h2>Ubicación</h2>
            <p>Ecuador, Machala. Calle Bolívar entre Avenida Vela, en una esquina frente al restaurante marineros</p>

            <h2>Horario</h2>
            <p>Abierto de lunes a domingo, de 9:00 a.m. a 10:00 p.m.</p>

            <h2>Promociones</h2>
            <div class="promo">
                <p>
                    Dependiendo a cómo tú proporciones tu horario de entrada y salida, al dar un dólar se equivale a una
                    hora o una hora y media. Con 3 dólares puedes estar toda la mañana experimentando la jugabilidad.
                </p>
            </div>
        </div>

        <div class="info">
            <h2>Ambiente Gaming</h2>
            <p>
                Contamos con ordenadores preparados para juegos pesados como LoL, Warzone y Fortnite. Disfruta de un
                espacio cómodo con asientos gamer y luz nocturna. También contamos con un aroma floral para ambientar.
            </p>
            <div class="gaming-image">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTH-XIFmvzpQVyJl7bR4VPcpP491SaAGTSmlg&s"
                    alt="Ambiente Gaming">
                <img class="circle-image"
                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXvJfPhuNJAVlZH9-p_Ix7qQQR6VfPEBryCQ&s"
                    alt="Ambiente Gaming Circular">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdBFZ2VO1NkgkVBDNAdUjl7y4FOIHCQpLt0EVBWn9MOxC4-rhkhsqLAL1EZThHIemL4hU&usqp=CAU"
                    alt="Ambiente Gaming 2">
            </div>
        </div>
        <div class="competencia">
            <h2>Competencias</h2>
            <p>
                Organizamos competencias inter-cantonales y nacionales, fortaleciendo la comunidad gaming de El Oro.
            </p>
        </div>
        <div class="contacto">
            <h2>Contactos</h2>
            <p>Correo: <a href="mailto:JARV_400@HOTMAIL.COM">JARV_400@HOTMAIL.COM</a></p>
            <p>Teléfono: <a href="tel:+593963047849">096 304 7849</a></p>
        </div>
        <a href="https://www.facebook.com/GamerLanDMachala/?locale=es_LA" class="button" target="_blank">Ver
            Publicidad</a>
    </div>
    <footer>
        <p>Elaborado por: Mathias Campoverde</p>
    </footer>

    <script>

        window.onload = function () {
            var modal = document.getElementById("myModal");
            var span = document.getElementsByClassName("close")[0];
            modal.style.display = "flex";
            span.onclick = function () {
                modal.style.display = "none";
            }
            window.onclick = function (event) {
                if (event.target == modal) {
                    modal.style.display = "none";
                }
            }
        };
    </script>
</b
