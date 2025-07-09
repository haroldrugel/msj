<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Z and F<3</title>
  <style>
    body {
      background: rgb(255, 255, 255);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      position: relative;
    }
    button {
      padding: 15px 30px;
      font-size: 1.2em;
      border: none;
      border-radius: 10px;
      background-color: #e4e4e4;
      color: #222222;
      cursor: pointer;
      transition: background-color 0.3s ease;
      z-index: 2;
    }
    button:hover {
      background-color: #ffffff;
    }
    .dedicatoria {
      position: absolute;
      bottom: 10px;
      font-size: 1.1em;
      color: #222222;
      text-align: center;
    }
    .mensaje {
      background-color: white;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      max-width: 600px;
      text-align: center;
      margin-top: 20px;
      display: none;
      z-index: 2;
    }
    .mensaje h1 {
      font-size: 1.8em;
      color: #222222;
    }
    .corazon {
      font-size: 2em;
      color: #ff4d4d;
      animation: latido 1s infinite;
    }
    @keyframes latido {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>
<body>

  <button id="btnMensaje" onclick="mostrarMensaje()">Ver mensaje</button>
  <div class="dedicatoria" id="dedicatoria">Para mi enojona</div>

  <div class="mensaje" id="mensaje">
    <div class="corazon">❤️</div>
    <h1>Somos muy jóvenes para prometernos un "Para Siempre",<br> pero llegaré contigo hasta donde tú me lo permitas.</h1>
  </div>

  <script>
    function mostrarMensaje() {
      document.getElementById('mensaje').style.display = 'block';
      document.getElementById('btnMensaje').style.display = 'none';
      document.getElementById('dedicatoria').style.display = 'none';
    }
  </script>

</body>
</html>
