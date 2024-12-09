<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tidalswimwear</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      background-color: #702359; /* Dark purple background */
    }
    header, footer {
      background-color: #E4ADD2;
      color: white;
      text-align: center;
      padding: 1em 0;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #FF38C0;
    }
    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #B058DC;
    }
    main {
      padding: 20px;
    }
    section {
      margin-bottom: 20px;
      background-color: #FECFF0;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    .dropdown-toggle {
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #FF38C0;
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      margin-bottom: 10px;
    }
    .dropdown-toggle:hover {
      background-color: #B058DC;
    }
    .product-container {
      display: none;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }
    .product {
      text-align: center;
      width: 200px;
    }
    .product img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }
    .product h3 {
      margin: 10px 0 5px;
    }
    .product p {
      margin: 5px 0;
    }
  </style>
</head>
<body>
  <header>
    <h1>👙 Tidalswimwear</h1>
    <p>We Love To See That!</p>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#products">Products</a>
    <a href="#about">About Us</a>
    <a href="#contact">Contact</a>
  </nav>
  <main>
    <section id="home">
      <h2>Welcome to Our Business</h2>
      <p>The trendiest swimwear & vintage swimwear all in one stop.</p>
    </section>
    <section id="services">
      <h2>Our Services</h2>
      <p>We provide authentic designs, high quality pieces for a very affordable price. As well as the personalization of each order to suit the customers body and likes &#x1F600;</p>
    </section>
    <section id="products">
      <div class="dropdown-toggle" onclick="toggleProducts()">
        <h2>Our Products</h2>
        <span>&#x25BC;</span> <!-- Down arrow -->
      </div>
      <div class="product-container">
        <!-- Sandy -->
        <div class="product">
          <img src="products/p1.jpg" alt="Sandy">
          <h3>Sandy</h3>
          <p>Two piece available in sizes S/M/L. Adjustable bra and stretchy bottom swim shorts.</p>
          <p><strong>R280</strong></p>
        </div>
        <!-- AMAHLE -->
        <div class="product">
          <img src="products/p2.jpg" alt="AMAHLE">
          <h3>AMAHLE</h3>
          <p>One-piece sexy stretchy swimsuit available in size S/M & XL.</p>
          <p><strong>R220</strong></p>
        </div>
        <!-- SBAHLE SET -->
        <div class="product">
          <img src="products/p3.jpg" alt="SBAHLE SET">
          <h3>SBAHLE SET</h3>
          <p>Three piece set. Classy swim wear available in size S/M/L.</p>
          <p><strong>R320</strong></p>
        </div>
        <!-- Wave -->
        <div class="product">
          <img src="products/p4.jpg" alt="Wave">
          <h3>Wave</h3>
          <p>Blue two piece set available in size S & L. Adjustable and stretchy.</p>
          <p><strong>R199</strong></p>
        </div>
        <!-- Bella -->
        <div class="product">
          <img src="products/p5.jpg" alt="Bella">
          <h3>Bella</h3>
          <p>One piece flower designed stretchy classy swimsuit. Available from size S - L.</p>
          <p><strong>R260</strong></p>
        </div>
        <!-- Emma -->
        <div class="product">
          <img src="products/p6.jpg" alt="Emma">
          <h3>Emma</h3>
          <p>Two pink set. Padded bra (adjustable) & stretchy bikini bottom only available in size M.</p>
          <p><strong>R180</strong></p>
        </div>
      </div>
    </section>
    <section id="about">
      <h2>About Us</h2>
      <p>Gcina</p>
    </section>
    <section id="contact">
      <h2>Contact Us</h2>
      <p>Email: gcinanatacha@gmail.com</p>
      <p>Phone: 0672183602</p>
      <p>Whatsapp: 0672183602</p>
      <p>IG: @Tidalswimwearr</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Tidalswimwear. All rights reserved.</p>
  </footer>

  <script>
    function toggleProducts() {
      const productContainer = document.querySelector('.product-container');
      productContainer.style.display = productContainer.style.display === 'none' || productContainer.style.display === '' 
        ? 'flex' 
        : 'none';
    }
  </script>
</body>
</html>

