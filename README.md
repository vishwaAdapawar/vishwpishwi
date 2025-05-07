<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VishwiPishwi – Khadi Clothing</title>
    <link rel="stylesheet" href="styles.css">
</head>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    text-align: center;
    background-color: #444;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

section {
    padding: 2rem;
    margin: 1rem;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.product {
    display: inline-block;
    width: 30%;
    margin: 1%;
    text-align: center;
    background-color: #f9f9f9;
    padding: 1rem;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.product img {
    width: 100%;
    height: auto;
    border-radius: 8px;
}

.product button {
    background-color: #333;
    color: #fff;
    border: none;
    padding: 0.5rem;
    border-radius: 5px;
    cursor: pointer;
}

.product button:hover {
    background-color: #555;
}

form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

form input, form textarea {
    padding: 0.5rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    width: 100%;
}

form button {
    background-color: #333;
    color: #fff;
    border: none;
    padding: 0.5rem;
    border-radius: 5px;
    cursor: pointer;
}

form button:hover {
    background-color: #555;
}

<body>
    <header>
        <h1>VishwiPishwi</h1>
        <p>Sustainable Khadi Clothing</p>
    </header>

    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#shop">Shop</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="home">
        <h2>Welcome to VishwiPishwi</h2>
        <p>Explore our exclusive collection of handcrafted khadi clothing.</p>
    </section>

    <section id="shop">
        <h2>Shop Our Collection</h2>
        <div class="product">
            <img src="images/kurta1.jpg" alt="Khadi Kurta">
            <h3>Khadi Kurta</h3>
            <p>₹1,200</p>
            <button onclick="addToCart('Khadi Kurta', 1200)">Add to Cart</button>
        </div>
        <div class="product">
            <img src="images/kurta2.jpg" alt="Khadi Dress">
            <h3>Khadi Dress</h3>
            <p>₹1,500</p>
            <button onclick="addToCart('Khadi Dress', 1500)">Add to Cart</button>
        </div>
        <div class="product">
            <img src="images/kurta3.jpg" alt="Khadi Top">
            <h3>Khadi Top</h3>
            <p>₹1,000</p>
            <button onclick="addToCart('Khadi Top', 1000)">Add to Cart</button>
        </div>
    </section>

    <section id="about">
        <h2>About VishwiPishwi</h2>
        <p>VishwiPishwi is dedicated to promoting sustainable fashion through handcrafted khadi clothing. Our pieces are made with love and care, ensuring quality and comfort.</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 VishwiPishwi</p>
    </footer>

    <script src="script.js"></script>
</body>
<body>
function addToCart(product, price) {
    alert(`${product} has been added to your cart. Price: ₹${price}`);
}

document.getElementById('contactForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Thank you for reaching out! We will get back to you shortly.');
});
</body>
</html>



