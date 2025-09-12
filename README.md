# voz visible
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Fondo con transición</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    background-color: #3498db; /* Fondo inicial azul */
    transition: background-color 2s ease; /* transición suave de 2 segundos */
  }

  /* Clase que cambia el fondo */
  .cambiar-fondo {
    background-color: #e74c3c; /* Fondo rojo */
  }
</style>
</head>
<body>

<h1>Hola, mira el fondo cambiar</h1>

<button id="btnFondo">Cambiar Fondo</button>

<script>
  const btn = document.getElementById('btnFondo');
  const body = document.body;

  btn.addEventListener('click', () => {
    body.classList.toggle('cambiar-fondo');
  });
</script>

</body>
</html>

