<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Music Landing Mockup</title>
<link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@700;900&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
<style>
  :root{
    --accent:#d9534f;
    --muted:#7a7a7a;
    --card-shadow: 0 12px 22px rgba(0,0,0,0.08);
    --card-shadow-2: 0 8px 18px rgba(0,0,0,0.06);
    --bg:#fff;
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family:"Open Sans",system-ui,Arial;
    color:#111;
    background:var(--bg);
    -webkit-font-smoothing:antialiased;
  }
  .wrap{max-width:1100px;margin:40px auto;padding:0 20px}
  /* Top headline */
  .headline{
    text-align:center;
    color:var(--accent);
    font-family:"Merriweather",serif;
    font-size:28px;
    margin-bottom:28px;
    font-weight:700;
  }
  /* Feature icons row */
  .features{
    display:flex;
    gap:30px;
    justify-content:space-between;
    align-items:flex-start;
    margin-bottom:42px;
    flex-wrap:wrap;
  }
  .feature{
    text-align:center;
    width:calc(25% - 22px);
    min-width:180px;
  }
  .feat-icon{
    width:92px;height:92px;border-radius:50%;
    background:#0e1720; display:flex; align-items:center; justify-content:center;
    margin:0 auto 12px; color:#69a3ff; font-weight:700; font-size:28px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.08);
  }
  .feature h4{margin:6px 0 6px;font-size:16px;font-weight:700}
  .feature p{margin:0;color:var(--muted);font-size:13px}
  /* Featured Guests */
  .section-title{
    text-align:center;
    color:var(--accent);
    font-family:"Merriweather",serif;
    font-size:26px;
    margin:36px 0;
    font-weight:700;
  }
  .guests{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:28px;
    margin-bottom:36px;
  }
  .card{
    background:#fff;padding:26px;border-radius:6px;box-shadow:var(--card-shadow);
    text-align:center; position:relative;
  }
  .avatar{
    width:110px;height:110px;border-radius:50%;overflow:hidden;margin:-70px auto 12px;
    border:6px solid #fff;box-shadow:0 6px 20px rgba(0,0,0,0.08);
    background:#eee;
  }
  .card h5{margin:6px 0 8px;font-family:"Merriweather",serif;font-size:18px}
  .card p{font-size:13px;color:var(--muted);line-height:1.45;margin:0 0 14px}
  .btn{
    display:inline-block;padding:8px 18px;border-radius:4px;background:var(--accent);
    color:#fff;font-weight:600;text-decoration:none;font-size:14px;box-shadow:var(--card-shadow-2);
  }
  /* "Buy What's New" */
  .buy-title{text-align:center;color:var(--accent);font-family:"Merriweather",serif;font-size:24px;margin:46px 0 20px;font-weight:700}
  .grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:22px;
    align-items:start;
  }
  .product{
    background:#fff;padding:0;border-radius:2px; overflow:hidden;
  }
  .product img{width:100%;height:180px;object-fit:cover;display:block}
  .product .meta{padding:12px 8px 18px}
  .product .meta h6{margin:0 0 6px;font-size:14px;font-weight:700}
  .product .meta span{display:block;color:var(--muted);font-size:13px}
  /* Responsive */
  @media (max-width:1000px){
    .features .feature{width:48%}
    .guests{grid-template-columns:repeat(2,1fr)}
    .grid{grid-template-columns:repeat(3,1fr)}
  }
  @media (max-width:640px){
    .features{gap:18px}
    .features .feature{width:100%}
    .guests{grid-template-columns:1fr}
    .grid{grid-template-columns:repeat(2,1fr)}
    .product img{height:150px}
  }
  @media (max-width:420px){
    .grid{grid-template-columns:1fr}
  }
</style>
</head>
<body>
  <main class="wrap">
    <h2 class="headline">Get ready for seamless online music</h2>
    <section class="features" aria-label="features">
      <div class="feature">
        <div class="feat-icon">↓</div>
        <h4>Offline mode</h4>
        <p>Save and listen anywhere.</p>
      </div>
      <div class="feature">
        <div class="feat-icon">HQ</div>
        <h4>High quality audio.</h4>
        <p>Enjoy the full range of sound.</p>
      </div>
      <div class="feature">
        <div class="feat-icon">ADS</div>
        <h4>No ads.</h4>
        <p>Enjoy nonstop music.</p>
      </div>
      <div class="feature">
        <div class="feat-icon">⏭</div>
        <h4>Unlimited skips.</h4>
        <p>Just tap skip.</p>
      </div>
    </section>
    <h3 class="section-title">Featured Guests</h3>
    <section class="guests" aria-label="featured guests">
      <!-- Card 1 -->
      <article class="card">
        <div class="avatar">
          <img src="https://images.unsplash.com/photo-1545996124-0b7a5c9b5182?auto=format&fit=crop&w=400&q=60" alt="Megan Smith">
        </div>
        <h5>Megan Smith</h5>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet, provident! Lorem ipsum dolor</p>
        <a class="btn" href="#">Register</a>
      </article>
      <!-- Card 2 -->
      <article class="card">
        <div class="avatar">
          <img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?auto=format&fit=crop&w=400&q=60" alt="Brooke Kagle">
        </div>
        <h5>Brooke Kagle</h5>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet, provident! Lorem ipsum dolor</p>
        <a class="btn" href="#">Register</a>
      </article>
      <!-- Card 3 -->
      <article class="card">
        <div class="avatar">
          <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?auto=format&fit=crop&w=400&q=60" alt="Philip Martin">
        </div>
        <h5>Philip Martin</h5>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet, provident! Lorem ipsum dolor</p>
        <a class="btn" href="#">Register</a>
      </article>
    </section>
    <h3 class="buy-title">BUY WHAT'S NEW</h3>
    <section class="grid" aria-label="products">
      <div class="product">
        <img src="https://picsum.photos/id/1060/800/600" alt="Garage Band 1">
        <div class="meta">
          <h6>Garage Band</h6>
          <span>Radio Station</span>
        </div>
      </div>
      <div class="product">
        <img src="https://picsum.photos/id/1011/800/600" alt="Garage Band 2">
        <div class="meta">
          <h6>Garage Band</h6>
          <span>Radio Station</span>
        </div>
      </div>
      <div class="product">
        <img src="https://picsum.photos/id/1025/800/600" alt="Garage Band 3">
        <div class="meta">
          <h6>Garage Band</h6>
          <span>Radio Station</span>
        </div>
      </div>
      <div class="product">
        <img src="https://picsum.photos/id/1040/800/600" alt="Garage Band 4">
        <div class="meta">
          <h6>Garage Band</h6>
          <span>Radio Station</span>
        </div>
      </div>
      <div class="product">
        <img src="https://picsum.photos/id/1050/800/600" alt="Garage Band 5">
        <div class="meta">
          <h6>Garage Band</h6>
          <span>Radio Station</span>
        </div>
      </div>
    </section>
  </main>
</body>
</html>
