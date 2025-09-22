<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Transición con logo 3 segundos</title>
  <style>
    body {
      margin: 0;
      background-color: #AEEAF7;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      transition: background-color 3s ease; /* 3 segundos */
      overflow: hidden;
    }

    img {
      width: 200px;
      transition: opacity 3s ease, transform 3s ease; /* 3 segundos */
    }

    .logo-out {
      opacity: 0;
      transform: translateY(-100px);
    }
  </style>
</head>
<body>

  <img id="logo" src="logo.png" alt="Logo" />

  <script>
    setTimeout(() => {
      // Cambiar fondo a blanco con transición de 3s
      document.body.style.backgroundColor = "#FFFFFF";

      // Añadir clase para animar logo durante 3s
      const logo = document.getElementById("logo");
      logo.classList.add("logo-out");

      // Quitar el logo del DOM después de 3s (termina animación)
      setTimeout(() => {
        logo.remove();
      }, 3000);
    }, 5000); // Espera 5 segundos antes de iniciar todo
  </script>

</body>
</html>

