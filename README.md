<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flipcart Clone</title>
    <link rel="stylesheet" href="ragul2.css">
</head>
<body>

    <header>
        <div class="logo">Flipcart</div>&emsp14;&emsp14;
        <input type="text" placeholder="Search for products" id="searchBox">
        <button onclick="search()">Search</button>&emsp14;&emsp14;
        <div class="cart" onclick="showCart()">🛒 <span id="cartCount">0</span></div>
    </header>

    <div class="products" id="productList">
        <!-- Products will be loaded here by JS -->
    </div>

    <div class="cart-details" id="cartDetails">
        <h3>Your Cart</h3>
        <ul id="cartItems"></ul>
        <button onclick="closeCart()">Close</button>
    </div>
    <!-- Add this at the end of <body> -->
<div id="addToCartPopup" class="modal">
    <div class="modal-content">
        <h3 id="popupProductName"></h3>
        <img id="popupProductImage" src="" alt="Product Image">
        <p id="popupProductPrice"></p>
        <button onclick="confirmAddToCart()">OK</button>
        <button onclick="cancelAddToCart()">Back</button>
    </div>
</div>

    <script src="ragul2.js"></script>
</body>
</html>
