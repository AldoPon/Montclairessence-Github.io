<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Montclairessence</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Roboto&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      background-color: #f5f5f5;
      color: #111;
    }

    header {
      background-color: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #ddd;
    }

    .logo {
      font-family: 'Playfair Display', serif;
      font-size: 32px;
      font-weight: 600;
      letter-spacing: 2px;
    }

    nav a {
      text-decoration: none;
      color: #111;
      margin-left: 20px;
      font-weight: 500;
    }

    .hero {
      background-image: url('https://images.unsplash.com/photo-1607083208528-6c5c1b8efc1f');
      background-size: cover;
      background-position: center;
      height: 80vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
      position: relative;
    }

    .hero::after {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0, 0, 0, 0.4);
    }

    .hero-content {
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: 56px;
      font-family: 'Playfair Display', serif;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 18px;
      margin-bottom: 20px;
    }

    .btn {
      background-color: #111;
      color: white;
      padding: 12px 24px;
      text-decoration: none;
      border-radius: 5px;
      font-size: 16px;
      transition: background 0.3s;
    }

    .btn:hover {
      background-color: #333;
    }

    footer {
      text-align: center;
      padding: 30px;
      background-color: white;
      font-size: 14px;
      color: #777;
      border-top: 1px solid #ddd;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">Montclairessence</div>
    <nav>
      <a href="#">Inicio</a>
      <a href="#">Perfumes</a>
      <a href="#">Nosotros</a>
      <a href="#">Contacto</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h1>La esencia del lujo</h1>
      <p>Descubre fragancias que definen tu elegancia</p>
      <a href="#perfumes" class="btn">Explorar colección</a>
    </div>
  </section>

  <footer>
    © 2025 Montclairessence · Todos los derechos reservados
  </footer>

</body>
</html>
