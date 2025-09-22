# <!DOCTYPE html>
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
    setTimeout(() => {
      document.body.classList.add('hidden'); // Inicia transición

      setTimeout(() => {
        // Redirige después de la transición
        window.location.href = "https://github.com/tu-usuario"; // <-- Cambia esto
      }, 1000); // Espera 1 segundo para terminar transición

    }, 1000); // Muestra pantalla azul por 1 segundo
  </script>
</body>
</html>

