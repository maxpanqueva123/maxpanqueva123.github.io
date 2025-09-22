<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Redirigiendo...</title>
  <style>
    body {
      margin: 0;
      background-color: #87CEFA; /* Azul celeste */
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      transition: opacity 1s ease;
      opacity: 1;
    }

    .hidden {
      opacity: 0;
    }

    h1 {
      color: white;
      font-family: sans-serif;
    }
  </style>
</head>
<body>
  <h1>Cargando...</h1>

  <script>
    // Espera 1 segundo para mostrar el fondo azul
    setTimeout(() => {
      document.body.classList.add('hidden'); // Aplica transición (fade out)

      // Luego de la transición, redirige automáticamente
      setTimeout(() => {
        window.location.href = "https://github.com/maxpanqueva123"; // Reemplaza con tu URL
      }, 1000); // Tiempo de transición
    }, 1000); // Tiempo inicial mostrando pantalla azul
  </script>
</body>
</html>


