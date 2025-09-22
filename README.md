<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Página con cambio de color</title>
  <style>
    body {
      margin: 0;
      background-color: #C4F1F9; /* hielo */
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      transition: background-color 1s ease;
    }

    img {
      width: 200px;
    }
  </style>
</head>
<body>

  <img src="logo.png" alt="Logo">

  <script>
    // Esperar 5 segundos y luego cambiar el fondo a blanco
    setTimeout(() => {
      document.body.style.backgroundColor = "#FFFFFF";
    }, 3000);
  </script>

</body>
</html>


