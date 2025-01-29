 
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            color: #d63384;
            padding: 50px;
        }
        .card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            display: inline-block;
            box-shadow: 0px 0px 15px rgba(0, 0, 0, 0.3);
            max-width: 450px;
            animation: fadeIn 1.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }
        h1 {
            font-size: 26px;
        }
        p {
            font-size: 18px;
            margin-bottom: 20px;
        }
        .heart {
            font-size: 50px;
            color: red;
            animation: heartbeat 1.5s infinite;
        }
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: all 0.3s ease;
        }
        .yes {
            background-color: #ff4d6d;
            color: white;
        }
        .no {
            background-color: #cccccc;
            color: black;
        }
        .yes:hover {
            background-color: #d63384;
            transform: scale(1.1);
        }
        .no:hover {
            background-color: #999999;
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <div class="card">
        <h1>¿Quieres ser mi San Valentín? ❤️</h1>
        <p>En un día como hoy, me gustaría poder decirte cuánto te amo. Tú eres mi felicidad. 💖</p>
        <p>No hay nadie en el mundo que haga latir mi corazón como tú. Eres mi vida entera, mi todo.</p>
        <p>Hoy quiero pedirte algo especial... <strong>¿Quieres ser mi San Valentín?</strong></p>
        <div class="heart">💖</div>
        <div class="buttons">
            <button class="yes" onclick="alert('¡Sabía que dirías que sí! ❤️ No sabes cuánto te amo.')">Sí</button>
            <button class="no" onclick="changeNoButton()">No</button>
        </div>
    </div>

    <script>
        function changeNoButton() {
            let noButton = document.querySelector('.no');
            noButton.innerText = "Quisiste decir que sí ❤️";
            noButton.style.backgroundColor = "#ff4d6d";
            noButton.style.color = "white";
            noButton.style.transform = "scale(1.1)";
            noButton.onclick = function() { 
                alert('¡Sabía que en el fondo querías decir que sí! ❤️'); 
            };
        }
    </script>

</body>
</html>
