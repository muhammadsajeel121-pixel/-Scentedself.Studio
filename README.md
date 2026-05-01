<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scentedself.studio | Luxury Candles</title>
    <style>
        :root { --cream: #FAF9F6; --brown: #5C4033; --tan: #D2B48C; }
        body { background-color: var(--cream); color: var(--brown); font-family: 'Playfair Display', serif; margin: 0; text-align: center; }
        .hero { padding: 80px 20px; background: white; border-bottom: 2px solid var(--tan); }
        .product-card { background: white; margin: 20px; padding: 25px; border-radius: 10px; border: 1px solid var(--tan); display: inline-block; width: 300px; vertical-align: top; }
        .price { font-size: 1.4rem; font-weight: bold; margin: 15px 0; color: #8B4513; }
        .order-btn { background-color: #25D366; color: white; padding: 12px 25px; text-decoration: none; border-radius: 30px; display: inline-block; font-weight: bold; border: none; cursor: pointer; }
        input, select { width: 80%; padding: 10px; margin: 10px 0; border: 1px solid var(--tan); border-radius: 5px; }
    </style>
</head>
<body>

<div class="hero">
    <h1>Scentedself.studio</h1>
    <p>Hand-poured Luxury from Sialkot</p>
</div>

<h2>Our Best Sellers</h2>

<div class="product-card">
    <h3>Daisy Bouquet (Bulk)</h3>
    <p>50 Pieces - Perfect for Events</p>
    <div class="price">Rs. 7,500</div>
    <button class="order-btn" onclick="sendOrder('Daisy Bouquet Bulk', '7500')">Order via WhatsApp</button>
</div>

<div class="product-card">
    <h3>Bridal Dress Candle</h3>
    <p>Elegant Wedding Favor</p>
    <div class="price">Rs. 750 (Single)</div>
    <button class="order-btn" onclick="sendOrder('Bridal Dress Candle', '750')">Order via WhatsApp</button>
</div>

<div class="product-card">
    <h3>Grand Bday Hamper</h3>
    <p>1 Jar, 1 Daisy, 2 Mini Bubbles</p>
    <div class="price">Rs. 3,079</div>
    <button class="order-btn" onclick="sendOrder('Grand Bday Hamper', '3079')">Order via WhatsApp</button>
</div>

<script>
    function sendOrder(product, price) {
        var name = prompt("Aapka Naam?");
        var color = prompt("Color choice? (Off-white, Pink, Sage Green, Yellow)");
        var qty = prompt("Quantity kitni chahiye?");
        
        var message = "Assalam-o-Alaikum! Mujhe order place karna hai:%0A%0A" +
                      "*Product:* " + product + "%0A" +
                      "*Price:* Rs. " + price + "%0A" +
                      "*Name:* " + name + "%0A" +
                      "*Color:* " + color + "%0A" +
                      "*Quantity:* " + qty + "%0A%0A" +
                      "Kindly confirm kardein.";
        
        window.open("https://wa.me/923XXXXXXXXX?text=" + message, '_blank');
    }
</script>

<div style="padding: 50px; background: var(--brown); color: white; margin-top: 50px;">
    <p>Customization: Name Sticker (Rs. 100) | Color Change (Rs. 50)</p>
    <p>© 2026 Scentedself.studio</p>
</div>

</body>
</html>
