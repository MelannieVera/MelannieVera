<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Cumpleaños</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffe6e6;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: red;
            font-size: 3em;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        .corazon {
            position: relative;
            width: 100px;
            height: 100px;
            background: red;
            transform: rotate(-45deg);
            margin: 10px;
            animation: latido 1s infinite;
        }
        .corazon::before,
        .corazon::after {
            content: "";
            position: absolute;
            width: 100px;
            height: 100px;
            background: red;
            border-radius: 50%;
        }
        .corazon::before {
            top: -50px;
            left: 0;
        }
        .corazon::after {
            left: 50px;
            top: 0;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes latido {
            0% { transform: scale(1) rotate(-45deg); }
            50% { transform: scale(1.2) rotate(-45deg); }
            100% { transform: scale(1) rotate(-45deg); }
        }
    </style>
</head>
<body>
    <h1>Feliz Cumpleaños, Te Amo</h1>
    <div class="corazon"></div>
</body>
</html>
