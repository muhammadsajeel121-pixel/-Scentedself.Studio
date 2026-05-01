<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scentedself.studio | Luxury Handmade Candles</title>
    <style>
        :root { --cream: #FAF9F6; --brown: #5C4033; --tan: #D2B48C; --dark-text: #3E2723; }
        body { background-color: var(--cream); color: var(--dark-text); font-family: 'Playfair Display', serif; margin: 0; text-align: center; }
        
        .hero { padding: 60px 20px; background: white; border-bottom: 2px solid var(--tan); }
        .hero h1 { font-size: 2.5rem; letter-spacing: 4px; margin-bottom: 10px; color: var(--brown); }
        
        .grid { display: flex; flex-wrap: wrap; justify-content: center; padding: 20px; }
        
        .product-card { 
            background: white; margin: 15px; padding: 15px; border-radius: 12px; 
            border: 1px solid var(--tan); width: 300px; transition: 0.3s; 
        }
        .product-card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.1); }
        
        .product-card img { 
            width: 100%; height: 250px; object-fit: cover; border-radius: 8px; margin-bottom: 15px; 
            background-color: #f0f0f0; /* Jab tak photo nahi aati, light gray dikhay ga */
        }
        
        .price { font-size: 1.3rem; font-weight: bold; margin: 10px 0; color: #8B4513; }
        
        .order-btn { 
            background-color: #25D366; color: white; padding: 12px 20px; 
            text-decoration: none; border-radius: 25px; display: inline-block; 
            font-weight: bold; border: none; cursor: pointer; width: 100%;
        }
        
        .footer { padding: 40px; background: var(--brown); color: white; margin-top: 50px; }
    </style>
</head>
<body>

<div class="hero">
    <h1>Scentedself.studio</h1>
    <p>Aesthetic & Hand-poured Luxury from Sialkot</p>
</div>

<h2>Shop Our Collection</h2>

<div class="grid">
    <div class="product-card">
        <img src="images/bridal_dress.jpg" alt="Bridal Dress Candle">
        <h3>Bridal Dress Candle</h3>
        <p>Special Wedding Favor</p>
        <div class="price">Rs. 750 (Single)</div>
        <button class="order-btn" onclick="sendOrder('Bridal Dress Candle', '750')">Order on WhatsApp</button>
    </div>

    <div class="product-card">
        <img src="images/daisy_flower.jpg" alt="Daisy Flower">
        <h3>Daisy Flower Candle</h3>
        <p>Available in Pastel Colors</p>
        <div class="price">Rs. 180</div>
        <button class="order-btn" onclick="sendOrder('Daisy Flower Candle', '180')">Order on WhatsApp</button>
    </div>

    <div class="product-card">
        <img src="images/bday_jar.jpg" alt="Birthday Jar">
        <h3>Birthday Jar (Sprinkles)</h3>
        <p>Customized Birthday Glow</p>
        <div class="price">Rs. 750</div>
        <button class="order-btn" onclick="sendOrder('Birthday Jar', '750')">Order on WhatsApp</button>
    </div>

    <div class="product-card">
        <img src="images/amber_jar.jpg" alt="Amber Jar">
        <h3>Luxury Amber Jar</h3>
        <p>Premium Scent & Lid</p>
        <div class="price">Rs. 2,500</div>
        <button class="order-btn" onclick="sendOrder('Amber Jar', '2500')">Order on WhatsApp</button>
    </div>
</div>

<script>
    function sendOrder(product, price) {
        var name = prompt("Aapka Naam?");
        var qty = prompt("Kitni candles chahiyein?");
        var color = prompt("Color choice? (Off-white, Sage Green, Pink, etc.)");
        
        // Apna WhatsApp number yahan likhein
        var myNumber = "923XXXXXXXXX"; 
        
        var message = "Assalam-o-Alaikum! Scentedself Studio, mujhe order place karna hai:%0A%0A" +
                      "*Product:* " + product + "%0A" +
                      "*Price:* Rs. " + price + "%0A" +
                      "*Name:* " + name + "%0A" +
                      "*Color:* " + color + "%0A" +
                      "*Quantity:* " + qty + "%0A%0A" +
                      "Kindly detail confirm kardein.";
        
        window.open("https://wa.me/" + myNumber + "?text=" + message, '_blank');
    }
</script>

<div class="footer">
    <p>Custom Name Sticker: Rs. 100 | Color Customization: Rs. 50</p>
    <p>Sialkot, Pakistan | Crafted by Rafay</p>
</div>

</body>
</html>
