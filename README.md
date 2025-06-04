<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Royal Indian Treasure Jewels Showroom</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet"/>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Open Sans', sans-serif;
      background-color: #fffefc;
      color: #333;
      line-height: 1.6;
    }
    header {
      background: linear-gradient(to right, #d4af37, #e8c76f);
      color: white;
      padding: 40px 20px;
      text-align: center;
      font-family: 'Playfair Display', serif;
    }
    header h1 {
      font-size: 3em;
      margin-bottom: 10px;
    }
    nav {
      background-color: #2f2f2f;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav a {
      color: white;
      padding: 15px 25px;
      text-decoration: none;
      font-weight: 600;
      transition: background 0.3s ease;
    }
    nav a:hover {
      background-color: #444;
      border-radius: 4px;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1603032483056-f90e7c3a3be7') center/cover no-repeat;
      height: 60vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
      font-size: 2.8em;
      font-weight: bold;
      text-shadow: 2px 2px 8px #000;
      font-family: 'Playfair Display', serif;
    }
    .section {
      padding: 60px 20px;
      text-align: center;
    }
    .section h2 {
      font-size: 2.5em;
      margin-bottom: 20px;
      color: #b3933a;
    }
    .section p {
      max-width: 800px;
      margin: auto;
      font-size: 1.1em;
      color: #555;
    }
    .about-section {
      background-color: #fef7e0;
      border-top: 3px solid #d4af37;
      border-bottom: 3px solid #d4af37;
    }
    .about-section p {
      font-size: 1.2em;
      color: #444;
      line-height: 1.8;
    }
    .logo-container {
      text-align: center;
      padding: 30px 0;
    }
    .logo-container img {
      max-width: 200px;
      height: auto;
    }
    .products {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
      margin-top: 20px;
    }
    .product-card {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      width: 280px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .product-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
    }
    .product-card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px 10px 0 0;
    }
    .product-card h3 {
      margin: 15px 0 5px;
      font-size: 1.3em;
      color: #444;
    }
    .product-card p {
      color: #b3933a;
      font-weight: bold;
      font-size: 1.1em;
      margin-bottom: 15px;
    }
    .tab-buttons {
      margin-bottom: 40px;
    }
    .tab-buttons button {
      background-color: #d4af37;
      border: none;
      color: white;
      padding: 12px 24px;
      margin: 5px;
      font-size: 1em;
      cursor: pointer;
      border-radius: 4px;
      transition: background 0.3s ease;
    }
    .tab-buttons button:hover {
      background-color: #b3933a;
    }
    .category {
      display: none;
    }
    .category.active {
      display: flex;
    }
    .contact-info {
      margin-top: 30px;
      font-size: 1.1em;
      line-height: 1.8;
    }
    footer {
      background-color: #222;
      color: white;
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
    }
    @media (max-width: 768px) {
      .hero {
        font-size: 2em;
        padding: 40px 20px;
        height: 40vh;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Royal Indian Treasure Jewels</h1>
    <p>Where Every Gem Tells a Story</p>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#about">About</a>
    <a href="#products">Collection</a>
    <a href="#contact">Contact</a>
  </nav>

  <div class="hero">
    Discover Your Sparkle
  </div>

  <section id="about" class="section about-section">
    <h2>About Us</h2>
    <p>The Royal Indian Treasure Jewels showcase India’s centuries-old tradition of fine jewelry. Our pieces reflect exquisite craftsmanship, featuring intricate gold and silver work with stunning diamonds, emeralds, rubies, and pearls. From heritage-inspired designs to modern elegance, every jewel tells a royal story.</p>
  </section>

  <div class="logo-container">
    <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\0V8XMXCU\IMG-20250530-WA0100[1].jpg" alt="Showroom Logo"/>
  </div>

  <section id="products" class="section">
    <h2>Featured Collection</h2>

    <div class="tab-buttons">
      <button onclick="showCategory('necklaces')">Necklaces</button>
      <button onclick="showCategory('earrings')">Earrings</button>
      <button onclick="showCategory('rings')">Rings</button>
    </div>

    <div id="necklaces" class="products category active">
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\0V8XMXCU\IMG-20250530-WA0079[1].jpg" alt="Gold Necklace">
        <h3>Necklace</h3>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\9JDXZFI4\IMG-20250530-WA0075[1].jpg" alt="Diamond Necklace">
        <h3>Diamond Necklace</h3>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\8UFW1CKZ\IMG-20250530-WA0033[1].jpg" alt="Bridal Necklace">
        <h3>Bridal Necklace</h3>
        <p>Rs.6,500</p>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\MIXKWN24\IMG-20250530-WA0037[1].jpg" alt="Temple Necklace">
        <h3>Temple Necklace</h3>
      </div>
    </div>

    <div id="earrings" class="products category">
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\8UFW1CKZ\IMG-20250530-WA0094[1].jpg" alt="Gold Earrings">
        <h3>Gold Earrings</h3>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\0V8XMXCU\IMG-20250530-WA0047[1].jpg" alt="Ruby Earrings">
        <h3>Ruby Earrings</h3>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\9JDXZFI4\IMG-20250530-WA0008[1].jpg" alt="Kundan Earrings">
        <h3>Kundan Earrings</h3>
      </div>
    </div>

    <div id="rings" class="products category">
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\MIXKWN24\IMG-20250530-WA0060[1].jpg" alt="Gold Ring">
        <h3>Gold Rings</h3>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\MIXKWN24\IMG-20250530-WA0063[1].jpg" alt="Emerald Ring">
        <h3>Emerald Ring</h3>
        <p>Rs. 85,000</p>
      </div>
      <div class="product-card">
        <img src="C:\Users\vshre\AppData\Local\Microsoft\Windows\INetCache\IE\0V8XMXCU\IMG-20250530-WA0084[1].jpg" alt="Antique Ring">
        <h3>Antique Ring</h3>
      </div>
    </div>
  </section>

  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <div class="contact-info">
      📍Building No./Flat No.:610/512, Maroofpur, Keshav Nagar, Fazullaganj, Lucknow, Uttar Pradesh 226020, India<br/>
      📞 +91-8081431205<br/>
      📧 vpiyush1814@gmail.com
    </div>
  </section>

  <footer>
    &copy; 2025 Royal Indian Treasure Jewels. All rights reserved.
  </footer>

  <script>
    function showCategory(category) {
      const categories = document.querySelectorAll('.category');
      categories.forEach(c => c.classList.remove('active'));
      document.getElementById(category).classList.add('active');
    }
  </script>
</body>
</html>
