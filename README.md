<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <style>
    /* Estilos generales */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f3f3f3;
    }

    /* Estilos para enlaces */
    a {
      text-decoration: none;
      color: #000;
      transition: color 0.3s;
    }

    a:hover {
      color: #b3843d;
    }

    /* Estilos para botones */
    .btn {
      background-color: #b3843d;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    /* Estilos para el encabezado */
    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #f9f9f9;
      padding: 20px;
      color: #000000;
      box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
    }

    .logo {
      display: flex;
      align-items: center;
    }

    .logo img {
      width: 80px;
      height: 80px;
      margin-right: 10px;
      border-radius: 50%;
    }

    .logo h1 {
      font-size: 24px;
    }

    .nav ul {
      list-style: none;
      display: flex;
      margin: 0;
      padding: 0;
    }

    .nav ul li {
      margin-right: 20px;
    }

    .nav a {
      text-decoration: none;
      color: #000000;
      font-weight: bold;
      transition: color 0.3s;
    }

    .nav a:hover {
      color: #b3843d;
    }

    /* Estilos para la sección Home */
    .home {
      width: 100%;
      height: 100vh;
      position: relative;
      background-image: url("C:\Users\user\Desktop\pagina-mafe\ban 1.jpg");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
    }

    .slideshow {
      position: relative;
      width: 100%;
      height: 100vh;
      overflow: hidden;
    }

    .slideshow-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .slideshow-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
      color: #000;
    }

    .slideshow-text h2 {
      font-size: 36px;
      margin-bottom: 10px;
    }

    .slideshow-text p {
      font-size: 18px;
    }

    /* Estilos para la sección Sobre Mí */
    .sobre-mi-contenido {
      display: flex;
      align-items: center;
      margin-top: 0px;
      background-color: #F3F3F3;
      padding: 100px 0;
    }

    .texto-sobre-mi {
      flex: 1;
      font-size: 18px;
      padding: 20px;
      background-color: rgba(225, 219, 219, 0.6);
      color: rgb(0, 0, 0);
      border-radius: 10px;
      margin-left: 20px;
    }

    .contenido-imagen img {
      width: 400px;
      height: 400px;
      margin-right: 20px;
    }

    .espacio-izquierda,
    .espacio-derecha {
      flex: 0.5;
    }

    .titulo-seccion {
      display: flex;
      align-items: center;
      margin-bottom: 30px;
      justify-content: center;
    }

    .titulo-seccion h2 {
      font-size: 28px;
      margin-right: 15px;
    }

    .linea-vertical {
      width: 1px;
      height: 40px;
      background-color: #333;
      margin-right: 15px;
    }

    /* Estilos para la sección de Servicios */
    .servicios {
      background-color: #fff;
      padding: 40px 0;
    }

    .contenedor-servicios {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }

    .servicio {
      width: calc(33.33% - 40px);
      margin: 20px;
      position: relative;
      overflow: hidden;
      border-radius: 10px;
      box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s;
    }

    .servicio img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      display: block;
      border-radius: 10px 10px 0 0;
    }

    .contenido-servicio {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.7);
      color: white;
      padding: 10px;
    }

    /* Estilos para el formulario de contacto */
    .formulario-contacto {
      padding: 40px;
      background-color: #F3F3F3;
      border-radius: 10px;
      margin-top: 20px;
    }

    .formulario-contacto h2 {
      font-size: 28px;
      margin-bottom: 20px;
    }

    .formulario-contacto label {
      display: block;
      font-weight: bold;
      margin-bottom: 5px;
    }

    .formulario-contacto input[type="text"],
    .formulario-contacto textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .formulario-contacto button {
      background-color: #b3843d;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    /* Estilos para el pie de página */
    .footer {
      text-align: center;
      padding: 20px;
      background-color: #f9f9f9;
    }
  </style>
  <title>Maria Fernanda Barbosa Torres - Abogada</title>
</head>
<body>
  <div class="header">
    <div class="logo">
      <img src="C:\Users\user\Desktop\pagina-mafe\Logo MB Abogados.pdf.png" alt="Logo">
      <h1>Maria Fernanda Barbosa Torres</h1>
    </div>
    <nav class="nav">
      <ul>
        <li><a href="#home">Inicio</a></li>
        <li><a href="#servicios">Servicios</a></li>
        <li><a href="#sobre-mi">Sobre mí</a></li>
        <li><a href="#contacto">Contacto</a></li>
        <li><a href="#solicitar-consulta">Solicitar Consulta</a></li>
      </ul>
    </nav>
  </div>

  <section id="home" class="home">
    <div class="slideshow">
      <div class="slideshow-image">
        <img src="C:\Users\user\Desktop\pagina-mafe\ban 1.jpg" alt="Slideshow">
      </div>
      <div class="slideshow-text">
        <h2>Tu abogada de confianza</h2>
        <p>Ofreciendo servicios legales de calidad...</p>
      </div>
    </div>
  </section>

  <section id="sobre-mi" class="sobre-mi">
    <div class="titulo-seccion">
      <h2>Sobre Mí</h2>
      <div class="linea-vertical"></div>
    </div>
    <div class="sobre-mi-contenido">
      <div class="espacio-izquierda"></div>
      <div class="contenido-imagen">
        <img src="C:\Users\user\Desktop\pagina-mafe\Tarjeta presentacion MB.png" alt="Imagen">
      </div>
      <div class="texto-sobre-mi">
        <p>¡Hola! Soy Maria Fernanda Barbosa Torres, una abogada apasionada de Colombia...</p>
        <p>Mi objetivo es brindar asesoría legal de calidad y responsable a mis clientes...</p>
        <p>Además de mi trabajo, disfruto del aprendizaje constante, la lectura y la conexión con colegas y amigos...</p>
      </div>
      <div class="espacio-derecha"></div>
    </div>
  </section>

  <section id="servicios" class="servicios">
    <div class="titulo-seccion">
      <h2>Servicios</h2>
      <div class="linea-vertical"></div>
    </div>
    <div class="contenedor-servicios">
      <div class="servicio">
        <img src="C:\Users\user\Desktop\pagina-mafe\ser 1.jpg" alt="Servicio 1">
        <div class="contenido-servicio">
          <h3>Asesoría Penal</h3>
          <p>Ofrecemos asesoría legal en casos penales para proteger tus derechos.</p>
          <a href="link_al_servicio_1" target="_blank" class="btn">Ver más</a>
        </div>
      </div>
      <div class="servicio">
        <img src="C:\Users\user\Desktop\pagina-mafe\ser 2.jpg" alt="Servicio 2">
        <div class="contenido-servicio">
          <h3>Asesoría Jurídica</h3>
          <p>Proporcionamos asesoramiento completo en diversas áreas legales.</p>
          <a href="link_al_servicio_2" target="_blank" class="btn">Ver más</a>
        </div>
      </div>
    </div>
  </section>

  <section id="contacto" class="contacto">
    <div class="informacion-contacto">
      <p>Gmail: mafea@gmail.com</p>
      <p>Teléfono: 1234567</p>
    </div>
    <div class="formulario-contacto">
      <h2>Solicitar Consulta</h2>
      <form id="consulta-form">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required>

        <label for="email">Email:</label>
        <input type="text" id="email" name="email" required>

        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje" rows="4" required></textarea>

        <button class="btn" type="submit">Enviar</button>
      </form>
    </div>
  </section>

  <footer class="footer">
    <p>&copy; 2023 Maria Fernanda Barbosa Torres. Todos los derechos reservados.</p>
  </footer>

  <script>
    const form = document.getElementById('consulta-form');
    form.addEventListener('submit', function (event) {
      event.preventDefault();
      // Agrega aquí el código para enviar el formulario
      // Puedes usar Fetch API o una biblioteca como axios
      // Una vez enviado, puedes mostrar un mensaje de éxito o realizar acciones adicionales
    });
  </script>
</body>
</html>
