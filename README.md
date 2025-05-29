<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Montclairessence</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Playfair Display', serif;
      background-color: #f8f7f4;
      color: #222;
    }
    header {
      background-color: #111;
      color: white;
      padding: 20px;
      text-align: center;
    }
    h1 {
      margin: 0;
      font-size: 2.5em;
      letter-spacing: 2px;
    }
    .container {
      max-width: 1100px;
      margin: auto;
      padding: 30px;
    }
    .product {
      background: white;
      border-radius: 20px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      margin-bottom: 40px;
      display: flex;
      flex-wrap: wrap;
      overflow: hidden;
    }
    .product img {
      width: 100%;
      max-width: 400px;
      object-fit: cover;
      flex: 1 1 40%;
    }
    .product-info {
      padding: 20px;
      flex: 1 1 60%;
    }
    .product-info h2 {
      margin-top: 0;
    }
    .buttons {
      margin-top: 20px;
    }
    .buttons a {
      text-decoration: none;
      margin-right: 15px;
      padding: 10px 20px;
      border-radius: 10px;
      background-color: #111;
      color: white;
      transition: 0.3s;
    }
    .buttons a:hover {
      background-color: #444;
    }
    footer {
      background-color: #111;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Montclairessence</h1>
    <p>Perfumería de lujo con esencia única</p>
  </header>

  <div class="container" id="product-list">
    <!-- Los productos se cargarán aquí -->
  </div>

  <footer>
    &copy; 2025 Montclairessence. Todos los derechos reservados.
  </footer>

  <script>
    const products = [
      {
        name: "Elixir Suprême",
        description: "Un aroma profundo, sensual y elegante.",
        image: "https://via.placeholder.com/400x500?text=Elixir+Suprême",
        paypalLink: "https://www.paypal.me/tuusuario/1000",
        mercadoPagoLink: "https://www.mercadopago.com.mx/link1",
        oxxoLink: "https://oxxo.com/pago1"
      },
      {
        name: "Nuit Dorée",
        description: "Notas doradas que brillan como el oro en la noche.",
        image: "https://via.placeholder.com/400x500?text=Nuit+Dorée",
        paypalLink: "https://www.paypal.me/tuusuario/1200",
        mercadoPagoLink: "https://www.mercadopago.com.mx/link2",
        oxxoLink: "https://oxxo.com/pago2"
      }
    ];

    const container = document.getElementById('product-list');

    products.forEach(product => {
      container.innerHTML += `
        <div class="product">
          <img src="${product.image}" alt="${product.name}">
          <div class="product-info">
            <h2>${product.name}</h2>
            <p>${product.description}</p>
            <div class="buttons">
              <a href="${product.paypalLink}" target="_blank">PayPal</a>
              <a href="${product.mercadoPagoLink}" target="_blank">MercadoPago</a>
              <a href="${product.oxxoLink}" target="_blank">OXXO</a>
            </div>
          </div>
        </div>
      `;
    });
  </script>
</body>
</html>
