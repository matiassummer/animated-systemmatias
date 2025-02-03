<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pregunta Especial</title>
    <style>
        #si {
            font-size: 16px;
            transition: font-size 0.3s ease;
        }
    </style>
</head>
<body>
    <h1>¿Quieres ser mi novia?</h1>
    <button id="si" onclick="responder('sí')">Sí</button>
    <button onclick="responder('no')">No</button>

    <p id="respuesta"></p>

    <script>
        function responder(respuesta) {
            if (respuesta === 'sí') {
                document.getElementById('respuesta').innerText = 'Te quiero mucho, rabanito 💖';
            } else {
                document.getElementById('si').style.fontSize = '30px'; // Aumentar tamaño del "Sí"
                document.getElementById('respuesta').innerText = ''; // Borrar mensaje
            }
        }
    </script>
</body>
</html>
