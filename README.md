<!-- HTML -->
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KPrime Travel Agency</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>

<!-- NAVBAR -->
<nav class="navbar">
  <div class="logo">KPrime Travel</div>
  <ul class="nav-links">
    <li><a href="#services">Services</a></li>
    <li><a href="#booking">Booking</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
  <a href="https://wa.me/254723718279" class="btn-primary"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
</nav>

<!-- HERO -->
<header class="hero">
  <div class="hero-content">
    <h1>Luxury Travel Experiences</h1>
    <p>Your gateway to exclusive hotel bookings, unforgettable tours, and tailored holiday packages.</p>
    <a href="https://wa.me/254723718279" class="btn-primary">Book Now</a>
    <a href="mailto:Kprime.travel.ke@gmail.com" class="btn-secondary">Email Us</a>
  </div>
</header>

<!-- SERVICES -->
<section id="services" class="services-section">
  <h2>Our Services</h2>
  <div class="services-grid">
    <div class="service-card">
      <i class="fa-solid fa-hotel fa-2x"></i>
      <h3>Hotel Bookings</h3>
      <p>Exclusive hotel deals in Diani and across Kenya for every budget.</p>
    </div>
    <div class="service-card">
      <i class="fa-solid fa-plane-departure fa-2x"></i>
      <h3>Holiday Packages</h3>
      <p>Custom packages for couples, families, and groups with unforgettable experiences.</p>
    </div>
    <div class="service-card">
      <i class="fa-solid fa-shuttle-space fa-2x"></i>
      <h3>Transfers</h3>
      <p>Reliable airport pickups and local transport to make your trip seamless.</p>
    </div>
    <div class="service-card">
      <i class="fa-solid fa-tree-city fa-2x"></i>
      <h3>Tours & Safaris</h3>
      <p>Curated safaris and tours to explore Kenya’s top destinations and hidden gems.</p>
    </div>
  </div>
</section>

<!-- BOOKING FORM -->
<section id="booking" class="booking-section">
  <h2>Request a Booking</h2>
  <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <input type="text" name="name" placeholder="Full Name" required>
    <input type="tel" name="phone" placeholder="Phone / WhatsApp" required>
    <input type="text" name="destination" placeholder="Destination / Hotel">
    <input type="text" name="dates" placeholder="Travel Dates">
    <textarea name="requests" placeholder="Special Requests"></textarea>
    <button type="submit">Submit Booking</button>
  </form>
</section>

<!-- CONTACT -->
<section id="contact" class="contact-section">
  <h2>Contact Us</h2>
  <p>Phone: +254 723 718279<br>Email: Kprime.travel.ke@gmail.com<br>Location: Kenya</p>
  <div class="contact-buttons">
    <a href="https://wa.me/254723718279" class="btn-primary"><i class="fa-brands fa-whatsapp"></i> WhatsApp</a>
    <a href="mailto:Kprime.travel.ke@gmail.com" class="btn-secondary">Email</a>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <p>&copy; 2026 KPrime Travel Agency. All Rights Reserved.</p>
</footer>

</body>
