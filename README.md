<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Simple E-Commerce Site</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="container">
      <h1>ShopMate</h1>
      <nav>
        <a href="#">Home</a>
        <a href="#">Products</a>
        <a href="#">Cart</a>
        <a href="#">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <h2>Featured Products</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="https://via.placeholder.com/150" alt="Product 1">
        <h3>Product Name</h3>
        <p>$19.99</p>
        <button>Add to Cart</button>
      </div>
      <div class="product-card">
        <img src="https://via.placeholder.com/150" alt="Product 2">
        <h3>Product Name</h3>
        <p>$24.99</p>
        <button>Add to Cart</button>
      </div>
      <!-- Add more product cards as needed -->
    </div>
  </main>

  <footer>
    <div class="container">
      <p>&copy; 2025 ShopMate. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

body {
  background-color: #f5f5f5;
  color: #333;
}

.container {
  width: 90%;
  max-width: 1200px;
  margin: 0 auto;
}

header {
  background-color: #222;
  color: white;
  padding: 20px 0;
}

header h1 {
  float: left;
}

nav {
  float: right;
}

nav a {
  color: white;
  margin-left: 20px;
  text-decoration: none;
}

header::after {
  content: "";
  display: table;
  clear: both;
}

main {
  padding: 40px 0;
}

.product-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.product-card {
  background: white;
  border: 1px solid #ddd;
  padding: 20px;
  flex: 1 1 calc(25% - 20px);
  min-width: 200px;
  text-align: center;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}

.product-card img {
  max-width: 100%;
  margin-bottom: 15px;
}

.product-card button {
  padding: 10px 20px;
  background: #007bff;
  color: white;
  border: none;
  cursor: pointer;
  border-radius: 4px;
}

.product-card button:hover {
  background: #0056b3;
}

footer {
  background-color: #222;
  color: white;
  text-align: center;
  padding: 20px 0;
  margin-top: 40px;
}
<div class="categories">
  <button onclick="filterProducts('all')">All</button>
  <button onclick="filterProducts('clothing')">Clothing</button>
  <button onclick="filterProducts('electronics')">Electronics</button>
</div>
<form class="login-form">
  <h2>Login</h2>
  <input type="text" placeholder="Email" required>
  <input type="password" placeholder="Password" required>
  <button type="submit">Login</button>
</form>
<input type="text" id="search" placeholder="Search products..." onkeyup="searchProducts()">
<button class="checkout-btn">Proceed to Checkout</button>
