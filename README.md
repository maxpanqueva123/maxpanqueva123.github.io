<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Transición con logo</title>
  <style>
    body {
      margin: 0;
      background-color: #AEEAF7; /* Fondo inicial celeste */
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      transition: background-color 1s ease;
      overflow: hidden; /* Evita scroll al mover el logo */
    }

    img {
      width: 200px;
      transition: opacity 1s ease, transform 1s ease;
    }

    /* Clase que activa la animación */
    .logo-out {
      opacity: 0;
      transform: translateY(-100px); /* Movimiento hacia arriba */
    }
  </style>
</head>
<body>

  <img id="logo" src="logo.png" alt="Logo">

  <script>
    setTimeout(() => {
      // Cambia el fondo a blanco
      document.body.style.backgroundColor = "#FFFFFF";

      // Anima el logo hacia arriba y lo desvanece
      const logo = document.getElementById("logo");
      logo.classList.add("logo-out");

      // Opcional: removerlo del DOM completamente después de la animación
      setTimeout(() => {
        logo.remove();
      }, 1000); // Espera a que termine la animación (1s)
    }, 5000);
  </script>

</body>
</html>

