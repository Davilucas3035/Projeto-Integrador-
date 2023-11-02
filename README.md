# Projeto-Integrador-
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matrix Effect</title>
    <link rel="stylesheet" href="Assets/css/styles.css">
</head>

<body>
    <div class="centered-text">Você foi hackeado(a) e seus dados estão sob vigilância!</div>
    <canvas id="matrix"></canvas>
    <script src="Assets/js/script.js"></script>
</body>

<head>
<style>
  body {
    animation: flash 2s infinite;
  }

  @keyframes flash {
    0% { background-color: black; }
    50% { background-color: red; }
    100% { background-color: black; }
  }
</style>
</head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<head>
    <style>
      body {
        animation: flash 2s infinite;
      }
    
      @keyframes flash {
        0% { background-color: black; }
        50% { background-color: red; }
        100% { background-color: black; }
      }
    </style>
    </head>
    <head>
        <style>
            @keyframes matrix-rain {
                100% { top: 500; }
                100% { top: 500px; }
            }
            .matrix-container {
                position: static;
                height: 500px;
                width: 100%;
                overflow: hidden;
            }
            .matrix-drop {
                position: absolute;
                font-size: 50px;
                font-weight: bold;
                color: rgb(255, 0, 0);
                animation: matrix-rain 2s linear infinite;
            }
        </style>
    </head>
    <body>
        <div class="matrix-container">
            <!-- Letras em quadrados com tamanho de fonte de 16px -->
        </div>
        <script>
            var chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
            for (var i = 0; i < 500; i++) {
                var drop = document.createElement("div");
                drop.className = "matrix-drop";
                drop.style.left = Math.random() * 100 + "%";
                drop.style.animationDelay = Math.random() * 2 + "s";
                drop.textContent = chars.charAt(Math.floor(Math.random() * chars.length));
                $(".matrix-container").append(drop);
            }
        </script>
    </body>
    </html>
