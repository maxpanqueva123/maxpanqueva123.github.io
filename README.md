<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Página con usuario en esquina</title>
  <style>
    body {
      margin: 0;
      background-color: #C4F1F9; /* Fondo que usa GitHub Pages */
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      transition: background-color 3s ease;
      overflow: hidden;
      position: relative;
    }

    img {
      width: 200px;
      transition: opacity 3s ease, transform 3s ease;
    }

    .logo-out {
      opacity: 0;
      transform: translateY(-100px);
    }

    #username {
      position: absolute;
      top: 10px;
      right: 10px;
      color: white;
      font-family: sans-serif;
      font-weight: bold;
      background: rgba(0,0,0,0.3);
      padding: 5px 10px;
      border-radius: 5px;
      user-select: none;
    }
  </style>
</head>
<body>

  <div id="username">maxpanqueva123</div>

  <img id="logo" src="logo.png" alt="Logo" />

  <script>
    setTimeout(() => {
      document.body.style.backgroundColor = "#FFFFFF";

      const logo = document.getElementById("logo");
      logo.classList.add("logo-out");

      setTimeout(() => {
        logo.remove();
      }, 3000);
    }, 5000);
  </script>

</body>
</html>
