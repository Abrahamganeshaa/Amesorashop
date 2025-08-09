<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Amesorashop</title>
  <meta name="description" content="Amesorashop — toko online sederhana. Produk berkualitas, pengiriman cepat.">
  <meta name="robots" content="index, follow">
  <!-- Open Graph (untuk preview jika dibagikan) -->
  <meta property="og:title" content="Amesorashop">
  <meta property="og:description" content="Amesorashop — toko online sederhana. Produk berkualitas, pengiriman cepat.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="">
  <meta property="og:image" content="https://via.placeholder.com/1200x630.png?text=Amesorashop">
  <link rel="icon" href="favicon.ico" type="image/x-icon">

  <style>
    :root{
      --bg1:#74ABE2;
      --bg2:#5563DE;
      --card: rgba(255,255,255,0.12);
      --card-hover: rgba(255,255,255,0.2);
      --accent: #FFD166;
      --glass: rgba(255,255,255,0.06);
      --maxwidth:1200px;
      color-scheme: light;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: Inter, "Segoe UI", Roboto, system-ui, -apple-system, "Helvetica Neue", Arial;
      background: linear-gradient(135deg,var(--bg1),var(--bg2));
      color:#fff;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
      padding-bottom:60px;
    }
    .wrap{
      max-width:var(--maxwidth);
      margin:0 auto;
      padding:24px;
    }

    header{
      text-align:center;
      padding:40px 12px;
      backdrop-filter: blur(4px);
    }
    header h1{
      font-size:2.2rem;
      letter-spacing:0.6px;
      margin-bottom:8px;
    }
    header p{
      opacity:0.95;
      margin:0;
    }

    nav{
      display:flex;
      justify-content:center;
      gap:12px;
      margin:22px 0;
      flex-wrap:wrap;
    }
    .nav-btn{
      text-decoration:none;
      color:#112;
      background:var(--accent);
      padding:10px 16px;
      border-radius:999px;
      font-weight:600;
      box-shadow: 0 6px 18px rgba(0,0,0,0.12);
      transition: transform .18s ease;
    }
    .nav-btn.secondary{
      background:transparent;
      color:#fff;
      border:1px solid rgba(255,255,255,0.18);
      padding:8px 14px;
    }
    .nav-btn:hover{ transform: translateY(-3px) }

    .hero{
      display:grid;
      grid-template-columns: 1fr;
      gap:20px;
      align-items:center;
      margin-bottom:28px;
    }
    .hero-card{
      background: linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.03));
      padding:18px;
      border-radius:14px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.18);
      display:flex;
      gap:18px;
      align-items:center;
    }
    .hero-card img{
      width:160px;
      height:108px;
      object-fit:cover;
      border-radius:10px;
      flex-shrink:0;
    }
    .hero-info h2{ margin:0 0 6px 0; font-size:1.2rem }
    .hero-info p{ margin:0; opacity:0.95 }

    .container{
      display:grid;
      grid-template-columns: repeat(auto-fit, minmax(240px,1fr));
      gap:18px;
      margin-top:18px;
    }
    .card{
      background:var(--card);
      padding:16px;
      border-radius:12px;
      text-align:center;
      transition: transform .18s ease, background .18s ease;
      display:flex;
      flex-direction:column;
      gap:12px;
    }
    .card:hover{
      background:var(--card-hover);
      transform: translateY(-6px);
    }
    .card img{
      width:100%;
      height:160px;
      object-fit:cover;
      border-radius:8px;
    }
    .product-title{ font-weight:700; color:#fff }
    .price{ font-weight:800; color:var(--accent); font-size:1.05rem }
    .btn-buy{
      background:var(--accent);
      border:none;
      padding:10px 14px;
      border-radius:10px;
      cursor:pointer;
      font-weight:700;
      box-shadow: 0 8px 20px rgba(0,0,0,0.12);
    }

    footer{
      margin-top:28px;
      text-align:center;
      padding:14px;
      border-radius:8px;
      background:var(--glass);
      position:fixed;
      left:0;
      right:0;
      bottom:0;
      display:flex;
      justify-content:center;
      align-items:center;
      gap:8px;
    }

    /* Responsive tweaks */
    @media(min-width:880px){
      .hero{ grid-template-columns: 1fr 420px; }
      header h1{ font-size:2.6rem }
    }
    @media(max-width:420px){
      .hero-card{ flex-direction:column; align-items:flex-start }
      .hero-card img{ width:100%; height:140px }
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Amesorashop</h1>
      <p>Toko online sederhana — produk pilihan & pengiriman cepat</p>
    </header>

    <nav>
      <a class="nav-btn" href="#produk">Produk</a>
      <a class="nav-btn secondary" href="#tentang">Tentang</a>
      <a class="nav-btn secondary" href="#kontak">Kontak</a>
    </nav>

    <section class="hero">
      <div class="hero-card" aria-label="Highlight produk">
        <img src="https://via.placeholder.com/480x320.png?text=Amesorashop" alt="Amesorashop">
        <div class="hero-info">
          <h2>Promo Spesial Minggu Ini</h2>
          <p>Dapatkan diskon untuk pembelian pertama — cek koleksi kami di bawah.</p>
        </div>
      </div>

      <aside style="padding:6px">
        <div style="background:rgba(255,255,255,0.04); padding:14px; border-radius:12px;">
          <h3 style="margin:0 0 8px 0">Newsletter</h3>
          <p style="margin:0 0 12px 0;opacity:0.95">Masukkan email untuk mendapat info diskon & produk baru</p>
          <form id="newsletter" onsubmit="event.preventDefault(); alert('Terima kasih! Email Anda telah didaftarkan.');">
            <input type="email" required placeholder="email@contoh.com" style="width:100%;padding:10px;border-radius:8px;border:none;margin-bottom:8px">
            <button type="submit" class="nav-btn" style="width:100%;">Daftar</button>
          </form>
        </div>
      </aside>
    </section>

    <main>
      <h2 id="produk" style="margin-top:6px">Produk Unggulan</h2>
      <div class="container" aria-live="polite">
        <!-- Item 1 -->
        <article class="card">
          <img src="https://via.placeholder.com/600x400.png?text=Produk+1" alt="Produk 1">
          <div>
            <div class="product-title">Produk 1</div>
            <div class="price">Rp 125.000</div>
            <p style="opacity:0.95;margin:8px 0 12px 0">Deskripsi singkat produk 1 yang menarik dan jelas.</p>
            <button class="btn-buy" onclick="beli('Produk 1',125000)">Beli</button>
          </div>
        </article>

        <!-- Item 2 -->
        <article class="card">
          <img src="https://via.placeholder.com/600x400.png?text=Produk+2" alt="Produk 2">
          <div>
            <div class="product-title">Produk 2</div>
            <div class="price">Rp 89.000</div>
            <p style="opacity:0.95;margin:8px 0 12px 0">Deskripsi singkat produk 2.</p>
            <button class="btn-buy" onclick="beli('Produk 2',89000)">Beli</button>
          </div>
        </article>

        <!-- Item 3 -->
        <article class="card">
          <img src="https://via.placeholder.com/600x400.png?text=Produk+3" alt="Produk 3">
          <div>
            <div class="product-title">Produk 3</div>
            <div class="price">Rp 230.000</div>
            <p style="opacity:0.95;margin:8px 0 12px 0">Deskripsi singkat produk 3.</p>
            <button class="btn-buy" onclick="beli('Produk 3',230000)">Beli</button>
          </div>
        </article>
      </div>

      <section id="tentang" style="margin-top:28px">
        <h2>Tentang Amesorashop</h2>
        <p style="opacity:0.95">Amesorashop adalah toko online sederhana untuk kebutuhan sehari-hari. Kami fokus pada kualitas dan layanan pelanggan.</p>
      </section>

      <section id="kontak" style="margin-top:18px">
        <h2>Kontak</h2>
        <p style="opacity:0.95">Email: <a href="mailto:contact@amesorashop.com" style="color:var(--accent);text-decoration:none">contact@amesorashop.com</a></p>
      </section>
    </main>
  </div>

  <footer>
    <small>&copy; <span id="year"></span> Amesorashop • Semua hak dilindungi.</small>
  </footer>

  <script>
    // tahun otomatis di footer
    document.getElementById('year').textContent = new Date().getFullYear();

    // fungsi beli (sederhana)
    function beli(nama, harga){
      const rupiah = harga.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".");
      if(confirm('Tambah "' + nama + '" ke keranjang? Harga: Rp ' + rupiah)){
        alert(nama + ' berhasil ditambahkan ke keranjang.\nLanjutkan ke pembayaran di proses berikutnya.');
      }
    }

    // smooth scroll for internal links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', function(e){
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if(target) target.scrollIntoView({behavior:'smooth', block:'start'});
      });
    });
  </script>
</body>
</html>
