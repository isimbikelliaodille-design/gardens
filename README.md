# gardens
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Gardens</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #333;
      background-color: #ffffff;
    }
    header {
      background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://empressofdirt.net/wp-content/uploads/fb-vegetable-garden-layout-ideas-v2.jpg') center/cover no-repeat;
      color: white;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }
    header h1 {
      font-size: 4rem;
      margin-bottom: 1rem;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.8);
    }
    header p {
      font-size: 1.5rem;
      max-width: 800px;
      margin-bottom: 2rem;
    }
    .btn {
      display: inline-block;
      background: #001f3f; /* dark blue */
      color: white;
      padding: 14px 32px;
      text-decoration: none;
      border-radius: 30px;
      font-size: 1.2rem;
      transition: background 0.3s, transform 0.2s;
    }
    .btn:hover {
      background: #0a2540;
      transform: translateY(-3px);
    }
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: #001f3f; /* dark blue */
      padding: 1rem 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.2);
    }
    nav .logo {
      font-size: 1.8rem;
      font-weight: bold;
      color: white;
    }
    nav ul {
      list-style: none;
      display: flex;
    }
    nav ul li {
      margin-left: 2.5rem;
    }
    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }
    nav ul li a:hover {
      color: #a0d8ef;
    }
    .menu-toggle {
      display: none;
      flex-direction: column;
      cursor: pointer;
    }
    .menu-toggle span {
      width: 28px;
      height: 3px;
      background: white;
      margin: 4px 0;
      transition: 0.3s;
    }
    section {
      padding: 100px 5%;
      max-width: 1300px;
      margin: 0 auto;
    }
    h2 {
      text-align: center;
      font-size: 3rem;
      margin-bottom: 3rem;
      color: #001f3f; /* dark blue */
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 2.5rem;
    }
    .card {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 8px 25px rgba(0, 31, 63, 0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      border: 1px solid #e0e7ff;
    }
    .card:hover {
      transform: translateY(-12px);
      box-shadow: 0 12px 35px rgba(0, 31, 63, 0.15);
    }
    .card img {
      width: 100%;
      height: 240px;
      object-fit: cover;
    }
    .card-content {
      padding: 1.8rem;
      text-align: center;
    }
    .card-content h3 {
      color: #001f3f;
      margin-bottom: 1rem;
    }
    .price {
      font-size: 1.4rem;
      font-weight: bold;
      color: #006400; /* dark green for prices */
      margin: 1rem 0;
    }
    .price-note {
      font-size: 0.9rem;
      color: #555;
      margin-top: 0.5rem;
    }
    form {
      max-width: 700px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
    }
    input, textarea {
      padding: 14px;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 1rem;
    }
    footer {
      background: #001f3f;
      color: white;
      text-align: center;
      padding: 3rem 1rem;
      margin-top: 4rem;
    }
    @media (max-width: 768px) {
      header h1 { font-size: 3rem; }
      nav ul {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 70px;
        left: 0;
        width: 100%;
        background: #001f3f;
        padding: 1.5rem 0;
      }
      nav ul.active { display: flex; }
      nav ul li { margin: 1.2rem 0; text-align: center; }
      .menu-toggle { display: flex; }
    }
  </style>
</head>
<body>

  <nav id="navbar">
    <div class="logo">Gardens</div>
    <ul id="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#activities">Activities</a></li>
      <li><a href="#boxes">Boxes</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div class="menu-toggle" onclick="toggleMenu()">
      <span></span><span></span><span></span>
    </div>
  </nav>

  <header id="home">
    <h1>Gardens</h1>
    <p>Passionate gardener helping beginners and enthusiasts create thriving, sustainable gardens with joy and expert tips.</p>
    <a href="#contact" class="btn">Get in Touch</a>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p style="max-width:900px; margin:0 auto; text-align:center; font-size:1.3rem;">
      Hello! I'm Isimbi Kellia Odille, dedicated to making gardening fun and accessible. From wonky veggies to wildflower meadows, I share advice, inspiration, and sustainable ideas for every level.
    </p>
  </section>

  <section id="activities">
    <h2>Activities & Resources</h2>
    <div class="grid">
      <div class="card">
        <img src="https://lovelygreens.com/wp-content/uploads/2021/02/february-veg-garden-jobs.jpg" alt="Open Gardens">
        <div class="card-content">
          <h3>Open Gardens</h3>
          <p>Explore beautiful community and private gardens for inspiration and ideas.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://i.etsystatic.com/30578449/r/il/39ac86/7145231042/il_1080xN.7145231042_21rn.jpg" alt="Monthly Checklist">
        <div class="card-content">
          <h3>Monthly Gardening Checklist</h3>
          <p>Seasonal tasks to keep your garden thriving all year round.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://randylemmon.com/wp-content/uploads/2026/02/greenhouse-gardening-tips-a-beginners-step-by-step-guide-768x432.png" alt="Greenhouse Tips">
        <div class="card-content">
          <h3>Greenhouse Tips</h3>
          <p>Expert advice for successful indoor growing and plant care.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://dengarden.com/.image/w_3840,q_auto:good,c_limit/MTc0Mjg5ODg2MTUxOTc2NDQ0/how-to-have-a-weed-free-low-maintenance-allotment.jpg?arena_f_auto" alt="Maintenance">
        <div class="card-content">
          <h3>Garden Maintenance Advice</h3>
          <p>Practical tips for pruning, weeding, soil health and more.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://lovelygreens.com/wp-content/uploads/2021/02/february-veg-garden-jobs.jpg" alt="Allotment">
        <div class="card-content">
          <h3>Allotment Jobs</h3>
          <p>Seasonal tasks tailored for plot holders and larger spaces.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://mommypotamus.com/wp-content/uploads/2020/04/gardening-for-beginners.jpg" alt="Competitions">
        <div class="card-content">
          <h3>Photographic Competitions</h3>
          <p>Share your garden photos and join fun seasonal challenges.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="boxes" style="background:#f8f9ff;">
    <h2>Our Gardening Boxes</h2>
    <div class="grid">
      <div class="card">
        <img src="https://static.independent.co.uk/2023/10/27/14/Oddbox.png" alt="Oddbox">
        <div class="card-content">
          <h3>Oddbox</h3>
          <p class="price">From £12.99 per box</p>
          <p>Wonky vegetables, weekly deliveries, blog, vegetable seeds.</p>
          <p class="price-note">+ £1.99 delivery (prices approx., vary by size)</p>
        </div>
      </div>
      <div class="card">
        <img src="https://joegardener.com/wp-content/uploads/2018/03/044-Featured-Image-708x466.jpg" alt="Flourish">
        <div class="card-content">
          <h3>Flourish</h3>
          <p class="price">£39.95 every 3 months</p>
          <p>Four seasonal boxes, seeds with trays, watering can, handmade soap.</p>
          <p class="price-note">(~£13.32/box equivalent)</p>
        </div>
      </div>
      <div class="card">
        <img src="https://mommypotamus.com/wp-content/uploads/2020/04/gardening-for-beginners.jpg" alt="Cottage">
        <div class="card-content">
          <h3>Cottage</h3>
          <p class="price">£19.99 per month</p>
          <p>Monthly surprises: wild flower seeds, fact cards, markers & twine.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://cdn.shopify.com/s/files/1/0573/3993/6868/files/Pretty_Wildflowers.jpg?v=1661452101" alt="Wildflower">
        <div class="card-content">
          <h3>Wildflower Wonder</h3>
          <p class="price">£14.99 per box</p>
          <p>Pollinator-friendly blooms, seasonal wildflower mixes and tips.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://randylemmon.com/wp-content/uploads/2026/02/greenhouse-gardening-tips-a-beginners-step-by-step-guide-768x432.png" alt="Greenhouse">
        <div class="card-content">
          <h3>Greenhouse Starter</h3>
          <p class="price">From £24.99 (or £9.99/month add-on)</p>
          <p>Indoor growing essentials, seed trays, tools and year-round tips.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://www.independent.co.uk/extras/indybest/food-drink/subscription-boxes/oddbox-review-wonky-fruit-veg-box-b2689210.html" alt="Custom">
        <div class="card-content">
          <h3>Custom / Corporate</h3>
          <p class="price">Contact for quote (from £50+)</p>
          <p>Tailored boxes for gifts, offices or events – get in touch!</p>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form id="contact-form">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="7" placeholder="Your Message" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
    <p style="text-align:center; margin-top:2.5rem; font-size:1.2rem;">
      Email: <a href="mailto:kelliaodilleisimbi@gmail.com">kelliaodilleisimbi@gmail.com</a><br>
      Phone: <a href="tel:+257994975952">07949 75952</a>
    </p>
  </section>

  <footer>
    <p>&copy; 2026 Isimbi Kellia Odille. All rights reserved. 🌱</p>
  </footer>

  <script>
    function toggleMenu() {
      document.getElementById('nav-links').classList.toggle('active');
    }

    window.addEventListener('scroll', () => {
      const nav = document.getElementById('navbar');
      nav.classList.toggle('scrolled', window.scrollY > 100);
    });

    document.getElementById('contact-form').addEventListener('submit', (e) => {
      e.preventDefault();
      alert('Thank you! I will get back to you soon.');
      e.target.reset();
    });

    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({ behavior: 'smooth' });
      });
    });
  </script>
</body>
</html>
