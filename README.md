!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulario de Incidencias</title>
</head>
<body>
  <h2>Registro de Incidencia</h2>
  <form action="#" method="POST" enctype="multipart/form-data">
    <!-- Información Básica -->
    <label for="title">Título de la incidencia:</label>
    <input type="text" id="title" name="title" required><br>

    <label for="name"> Piso y habitación:</label>
    <input type="text" id="name" name="name" required><br>

    <label for="email">Correo electrónico:</label>
    <input type="email" id="email" name="email" required><br>

    <!-- Detalles de la Incidencia -->
    <label for="type">Tipo de incidencia:</label>
    <select id="type" name="type" required>
      <option value="electricidad">Electricidad</option>
      <option value="plomeria">Plomería</option>
      <option value="otros">Otros</option>
    </select><br>

    <label for="description">Descripción del problema:</label>
    <textarea id="description" name="description" rows="4" required></textarea><br>

    <!-- Adjuntos -->
    <label for="images">Subir imágenes:</label>
    <input type="file" id="images" name="images[]" accept="image/*" multiple><br>

    <!-- Confirmación -->
    <label for="terms">
      <input type="checkbox" id="terms" name="terms" required>
      Confirmo que la información es correcta.
    </label><br>

    <!-- Botones -->
    <button type="submit">Enviar</button>
  </form>
</body>
</html>
