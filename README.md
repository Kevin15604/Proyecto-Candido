# Proyecto-Candido
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Conciencia sobre la Violencia de Género</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fefefe;
        }

        header {
            background-color: #880e4f;
            color: white;
            padding: 20px;
            text-align: center;
        }

        main {
            padding: 20px;
            max-width: 1000px;
            margin: auto;
        }

        section {
            background-color: white;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 10px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        img, video {
            width: 100%;
            border-radius: 10px;
            margin-top: 10px;
        }

        input, textarea, button {
            width: 100%;
            padding: 10px;
            margin: 8px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1em;
        }

        button {
            background-color: #880e4f;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #ad1457;
        }

        .center {
            text-align: center;
        }

        #score {
            font-size: 2em;
            margin-top: 10px;
        }

        @media screen and (max-width: 768px) {
            body {
                padding: 10px;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Alza la Voz</h1>
    <p>Concientización contra la Violencia de Género</p>
</header>

<main>

    <!-- Sección multimedia -->
    <section>
        <h2>¿Qué es la violencia de género?</h2>
        <p>La violencia de género es cualquier acto dañino basado en el género que causa daño o sufrimiento físico, sexual o psicológico.</p>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/VG_day_against_gender_violence_purple_hand.jpg/800px-VG_day_against_gender_violence_purple_hand.jpg" alt="Imagen contra la violencia de género">
        <video controls>
            <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
            Tu navegador no soporta el video.
        </video>
    </section>

    <!-- Formulario de registro -->
    <section>
        <h2>Regístrate para unirte</h2>
        <form>
            <input type="text" placeholder="Nombre completo" required>
            <input type="email" placeholder="Correo electrónico" required>
            <textarea placeholder="¿Por qué deseas unirte a la causa?" rows="4" required></textarea>
            <button type="submit">Registrarse</button>
        </form>
    </section>

    <!-- Noticias -->
    <section>
        <h2>Últimas Noticias</h2>
        <article>
            <h3>Ley de protección integral a víctimas</h3>
            <p>Se promulgó una nueva ley que refuerza la atención y protección a mujeres víctimas de violencia de género.</p>
        </article>
        <article>
            <h3>Campañas de concientización en escuelas</h3>
            <p>Organizaciones civiles inician talleres educativos en escuelas secundarias para prevenir la violencia de género desde temprana edad.</p>
        </article>
    </section>

    <!-- Videojuego sencillo -->
    <section>
        <h2>Juego: ¡Actúa contra la violencia!</h2>
        <p class="center">Haz clic en el botón para representar acciones positivas. ¡Suma apoyos!</p>
        <div class="center">
            <button onclick="incrementarPuntos()">¡Actuar!</button>
            <div id="score">0</div>
        </div>
    </section>

</main>

<script>
    let puntos = 0;
    function incrementarPuntos() {
        puntos++;
        document.getElementById("score").innerText = puntos;
    }
</script>

</body>
</html>
