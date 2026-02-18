<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KPrime Travel Agency</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
/* GENERAL STYLES */
body {margin:0;font-family:Arial,Helvetica,sans-serif;background:#f4f6fb;color:#222;}
a {text-decoration:none;}
h2,h3{margin-bottom:15px;}
section {padding:70px 20px;max-width:1200px;margin:auto;}

/* NAVBAR */
nav {position:fixed;top:0;width:100%;background:white;box-shadow:0 2px 10px rgba(0,0,0,.08);padding:15px 30px;display:flex;justify-content:space-between;align-items:center;z-index:1000;}
nav b {font-size:20px;color:#0a2a43;}
nav a {color:#333;margin-left:20px;font-weight:600;transition:.3s;}
nav a:hover{color:#0f6ea8;}
.btn-primary {background:#0f6ea8;color:white;padding:10px 20px;border-radius:5px;transition:.3s;}
.btn-primary:hover{background:#095580;}
.btn-secondary {background:#555;color:white;padding:10px 20px;border-radius:5px;transition:.3s;}
.btn-secondary:hover{background:#333;}

/* HERO */
header {padding:140px 20px 100px;text-align:center;background:linear-gradient(rgba(10,42,67,.7),rgba(10,42,67,.7)),url('');background-size:cover;background-position:center;color:white;}
header h1 {font-size:48px;margin-bottom:10px;}
header p {font-size:20px;opacity:.95;}

/* CARDS */
.grid {display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:25px;}
.card {background:white;padding:30px;border-radius:14px;box-shadow:0 8px 22px rgba(0,0,0,.07);text-align:center;transition:.3s;}
.card:hover{transform:translateY(-5px);box-shadow:0 12px 30px rgba(0,0,0,.15);}
.card i {font-size:36px;color:#0f6ea8;margin-bottom:10px;}

/* FORMS */
form {background:white;padding:35px;border-radius:14px;box-shadow:0 8px 22px rgba(0,0,0,.07);max-width:600px;margin:auto;display:flex;flex-direction:column;gap:15px;}
input,textarea {width:100%;padding:14px;margin:10px 0;border-radius:8px;border:1px solid #ddd;font-size:15px;}
button {background:#0f6ea8;color:white;padding:15px;border:none;width:100%;border-radius:8px;font-size:16px;font-weight:bold;cursor:pointer;transition:.3s;}
button:hover{background:#095580;}

/* HOTEL GALLERY */
.gallery {display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:20px;margin-top:30px;}
.hotel-card {position:relative;border-radius:12px;overflow:hidden;box-shadow:0 8px 22px rgba(0,0,0,.07);transition:.3s;background:#ddd;height:220px;display:flex;align-items:center;justify-content:center;font-weight:bold;font-size:18px;color:#555;}

/* REVIEWS */
.reviews {background:#f0f4f8;padding:50px 20px;}
.review-card {background:white;padding:20px;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,.08);margin-bottom:20px;}
.review-card p{font-style:italic;}
.review-card b{display:block;margin-bottom:8px;color:#0f6ea8;}

/* FOOTER */
footer {background:#0a2a43;color:white;text-align:center;padding:40px 20px;}

/* WHATSAPP BUTTON */
.whatsapp {position:fixed;bottom:18px;right:18px;background:#25D366;color:white;padding:16px 18px;border-radius:50%;font-size:22px;text-decoration:none;box-shadow:0 6px 16px rgba(0,0,0,.3);}

/* RESPONSIVE */
@media(max-width:768px){header h1{font-size:36px;}nav{flex-direction:column;gap:10px;}}
</style>
</head>
<body>

<!-- NAVBAR -->
<nav>
<b>KPrime Travel</b>
<div>
<a href="#services">Services</a>
<a href="#booking">Booking</a>
<a href="#gallery">Hotels</a>
<a href="#reviews">Reviews</a>
<a href="#contact">Contact</a>
</div>
<a class="btn-primary" href="https://wa.me/254723718279"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
</nav>

<!-- HERO -->
<header>
<h1>KPrime Travel Agency</h1>
<p>Luxury hotel bookings, holidays & unforgettable travel experiences</p>
<a class="btn-primary" href="https://wa.me/254723718279">Book Now on WhatsApp</a>
<a class="btn-secondary" href="mailto:Kprime.travel.ke@gmail.com">Email Us</a>
</header>

<!-- SERVICES -->
<section id="services">
<h2>Our Services</h2>
<div class="grid">
<div class="card"><i class="fa-solid fa-hotel"></i><h3>Hotel Bookings</h3><p>Exclusive rates for top hotels in Diani and across Kenya.</p></div>
<div class="card"><i class="fa-solid fa-plane-departure"></i><h3>Holiday Packages</h3><p>Romantic, family & custom travel packages tailored for you.</p></div>
<div class="card"><i class="fa-solid fa-shuttle-space"></i><h3>Transfers</h3><p>Reliable airport pickups and transport arrangements.</p></div>
<div class="card"><i class="fa-solid fa-tree-city"></i><h3>Tours & Safaris</h3><p>Curated adventures and Kenyan safari experiences.</p></div>
</div>
</section>

<!-- BOOKING FORM -->
<section id="booking">
<h2>Request Booking</h2>
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
<input type="text" name="name" placeholder="Your Name" required>
<input type="tel" name="phone" placeholder="Phone / WhatsApp" required>
<input type="text" name="destination" placeholder="Destination / Hotel">
<input type="text" name="dates" placeholder="Travel Dates">
<textarea name="requests" placeholder="Special Requests"></textarea>
<button type="submit">Submit Request</button>
</form>
</section>

<!-- HOTEL GALLERY -->
<section id="gallery">
<h2>Hotel Gallery</h2>
<div class="gallery">
<div class="hotel-card">Your Hotel Name Here</div>
<div class="hotel-card">Your Hotel Name Here</div>
<div class="hotel-card">Your Hotel Name Here</div>
</div>
</section>

<!-- CLIENT REVIEWS FORM -->
<section id="reviews">
<h2>Write a Review</h2>
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
<input type="text" name="name" placeholder="Your Name" required>
<textarea name="review" placeholder="Write your review here" required></textarea>
<button type="submit">Submit Review</button>
</form>
</section>

<!-- CONTACT -->
<section id="contact" style="text-align:center">
<h2>Contact</h2>
<p><b>Phone:</b> +254 723 718279</p>
<p><b>Email:</b> Kprime.travel.ke@gmail.com</p>
<p><b>Location:</b> Kenya</p>
</section>

<!-- FOOTER -->
<footer>
© 2026 KPrime Travel Agency — Premium Travel Services
</footer>

<!-- WHATSAPP -->
<a class="whatsapp" href="https://wa.me/254723718279">💬</a>

</body>
</html>
