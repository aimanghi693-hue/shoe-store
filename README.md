# shoe-store
High-end shoes, Adidas, Nike, Louis Vuitton, sold worldwide.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Luxury Shoes Bahrain</title>
  <style>
    body { margin:0; font-family: Arial, sans-serif; background:#f5f5f5; }
    header { background:#111; color:#fff; padding:15px; text-align:center; }
    nav { display:flex; justify-content:center; gap:20px; background:#222; padding:10px; }
    nav a { color:#fff; text-decoration:none; font-weight:bold; }
    .lang { position:absolute; right:15px; top:15px; }
    .hero { background:url('https://images.unsplash.com/photo-1542291026-7eec264c27ff') center/cover; color:white; text-align:center; padding:80px 20px; }
    .hero h1 { font-size:40px; }
    .container { padding:20px; }
    .grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(200px,1fr)); gap:20px; }
    .card { background:white; border-radius:10px; padding:15px; text-align:center; box-shadow:0 2px 5px rgba(0,0,0,0.1); }
    .card img { width:100%; border-radius:10px; }
    .price { color:green; font-size:18px; margin:10px 0; }
    .btn { background:#000; color:#fff; padding:10px; border:none; cursor:pointer; border-radius:5px; }
    .badge { color:orange; font-size:14px; }
    footer { background:#111; color:#fff; text-align:center; padding:15px; margin-top:20px; }
  </style>
</head>
<body>

<header>
  <h2>Luxury Shoes Bahrain</h2>
  <div class="lang">
    <button onclick="setLang('en')">EN</button>
    <button onclick="setLang('ar')">AR</button>
  </div>
</header>

<nav>
  <a href="#">Men</a>
  <a href="#">Women</a>
  <a href="#">Sports</a>
  <a href="#">Kids</a>
</nav>

<section class="hero">
  <h1 id="title">Premium Collection 2026</h1>
  <p id="subtitle">High Quality | Best Prices | Fast Delivery in Bahrain</p>
</section>

<div class="container">
  <h2>🔥 Best Sellers</h2>
  <div class="grid">

    <div class="card">
      <span class="badge">🔥 120+ sold</span>
      <img src="https://images.unsplash.com/photo-1600185365483-26d7a4cc7519">
      <h3>Men Sneakers</h3>
      <p class="price">15 BD</p>
      <button class="btn" onclick="order('Men Sneakers')">Order via WhatsApp</button>
    </div>

    <div class="card">
      <span class="badge">🔥 90+ sold</span>
      <img src="https://images.unsplash.com/photo-1525966222134-fcfa99b8ae77">
      <h3>Women Shoes</h3>
      <p class="price">12 BD</p>
      <button class="btn" onclick="order('Women Shoes')">Order via WhatsApp</button>
    </div>

    <div class="card">
      <span class="badge">🔥 150+ sold</span>
      <img src="https://images.unsplash.com/photo-1519741497674-611481863552">
      <h3>Sports Shoes</h3>
      <p class="price">18 BD</p>
      <button class="btn" onclick="order('Sports Shoes')">Order via WhatsApp</button>
    </div>

    <div class="card">
      <span class="badge">🔥 70+ sold</span>
      <img src="https://images.unsplash.com/photo-1584735175315-9d5df23be620">
      <h3>Kids Shoes</h3>
      <p class="price">10 BD</p>
      <button class="btn" onclick="order('Kids Shoes')">Order via WhatsApp</button>
    </div>

  </div>
</div>

<footer>
  <p>📞 WhatsApp: +447401928886</p>
</footer>

<script>
function order(product){
  var phone = '973XXXXXXXX'; // 替换你的号码
  var message = 'Hello, I want to order: ' + product;
  var url = 'https://wa.me/' + phone + '?text=' + encodeURIComponent(message);
  window.open(url, '_blank');
}

function setLang(lang){
  if(lang === 'ar'){
    document.getElementById('title').innerText = 'مجموعة 2026 المميزة';
    document.getElementById('subtitle').innerText = 'جودة عالية | أفضل الأسعار | توصيل سريع';
  } else {
    document.getElementById('title').innerText = 'Premium Collection 2026';
    document.getElementById('subtitle').innerText = 'High Quality | Best Prices | Fast Delivery in Bahrain';
  }
}
</script>

</body>
</html>
