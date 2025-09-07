<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>لبنیات طبیعی</title>
  <style>
    /* --- ریست ساده --- */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Tahoma', sans-serif; }
    body { background-color: #fdfaf6; color: #333; line-height: 1.6; }

    /* --- هدر --- */
    header { background-color: #a2d5c6; padding: 20px 0; text-align: center; }
    header h1 { font-size: 2.2rem; color: #fff; }
    nav { margin-top: 10px; }
    nav a {
      text-decoration: none;
      color: #fff;
      margin: 0 15px;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover { color: #333; }

    /* --- بخش اصلی --- */
    .hero {
      background: url('https://images.unsplash.com/photo-1604908177525-2f85a6d5480d?auto=format&fit=crop&w=1350&q=80') center/cover no-repeat;
      height: 60vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
      font-size: 2rem;
    }

    /* --- محصولات --- */
    .products { display: flex; flex-wrap: wrap; justify-content: center; padding: 40px 20px; gap: 20px; }
    .product-card {
      background-color: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      overflow: hidden;
      width: 250px;
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .product-card:hover { transform: translateY(-5px); box-shadow: 0 8px 20px rgba(0,0,0,0.2); }
    .product-card img { width: 100%; height: 180px; object-fit: cover; }
    .product-card h3 { margin: 10px 0; color: #2a7f62; }
    .product-card p { margin: 5px 0 15px; color: #555; }
    .product-card button {
      background-color: #2a7f62;
      color: #fff;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    .product-card button:hover { background-color: #1e5a44; }

    /* --- درباره ما --- */
    .about { background-color: #e9f4f1; padding: 60px 20px; text-align: center; }
    .about h2 { color: #2a7f62; margin-bottom: 20px; }
    .about p { max-width: 700px; margin: 0 auto; color: #555; }

    /* --- تماس با ما --- */
    .contact { padding: 60px 20px; text-align: center; }
    .contact h2 { color: #2a7f62; margin-bottom: 20px; }
    .contact form { max-width: 500px; margin: 0 auto; display: flex; flex-direction: column; gap: 15px; }
    .contact input, .contact textarea {
      padding: 10px; border: 1px solid #ccc; border-radius: 8px; font-size: 1rem;
    }
    .contact button {
      background-color: #2a7f62;
      color: #fff;
      border: none;
      padding: 12px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
      transition: background-color 0.3s;
    }
    .contact button:hover { background-color: #1e5a44; }

    /* --- فوتر --- */
    footer {
      background-color: #a2d5c6;
      color: #fff;
      text-align: center;
      padding: 20px 0;
      margin-top: 40px;
    }

    @media(max-width: 768px){
      .products { flex-direction: column; align-items: center; }
    }
  </style>
</head>
<body>

  <!-- هدر -->
  <header>
    <h1>لبنیات طبیعی</h1>
    <nav>
      <a href="#home">خانه</a>
      <a href="#products">محصولات</a>
      <a href="#about">درباره ما</a>
      <a href="#contact">تماس با ما</a>
    </nav>
  </header>

  <!-- بخش اصلی -->
  <section class="hero" id="home">
    تازه و سالم، مستقیم از مزرعه!
  </section>

  <!-- محصولات -->
  <section class="products" id="products">
    <div class="product-card">
      <img src="https://images.unsplash.com/photo-1604908177525-2f85a6d5480d?auto=format&fit=crop&w=400&q=80" alt="شیر تازه">
      <h3>شیر تازه</h3>
      <p>قیمت: 25,000 تومان</p>
      <button>خرید</button>
    </div>
    <div class="product-card">
      <img src="https://images.unsplash.com/photo-1617196035487-896d2b2b44b3?auto=format&fit=crop&w=400&q=80" alt="ماست طبیعی">
      <h3>ماست طبیعی</h3>
      <p>قیمت: 18,000 تومان</p>
      <button>خرید</button>
    </div>
    <div class="product-card">
      <img src="https://images.unsplash.com/photo-1592906200846-1f71a6f8b3c3?auto=format&fit=crop&w=400&q=80" alt="پنیر محلی">
      <h3>پنیر محلی</h3>
      <p>قیمت: 30,000 تومان</p>
      <button>خرید</button>
    </div>
  </section>

  <!-- درباره ما -->
  <section class="about" id="about">
    <h2>درباره ما</h2>
    <p>
      ما در لبنیات طبیعی به سلامت و کیفیت اهمیت می‌دهیم. محصولات ما مستقیماً از مزرعه‌های سالم و به صورت طبیعی تهیه می‌شوند تا بهترین طعم و ارزش غذایی را برای شما فراهم کنیم.
    </p>
  </section>

  <!-- تماس با ما -->
  <section class="contact" id="contact">
    <h2>تماس با ما</h2>
    <form>
      <input type="text" placeholder="نام شما" required>
      <input type="email" placeholder="ایمیل شما" required>
      <textarea rows="5" placeholder="پیام شما" required></textarea>
      <button type="submit">ارسال پیام</button>
    </form>
  </section>

  <!-- فوتر -->
  <footer>
    &copy; 2025 لبنیات طبیعی. تمام حقوق محفوظ است.
  </footer>

</body>
</html>
