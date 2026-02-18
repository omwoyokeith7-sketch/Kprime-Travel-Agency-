<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kprime Travel Agency</title>

<style>
body{margin:0;font-family:Segoe UI;background:#f4f6fb;color:#111}
header{background:linear-gradient(120deg,#081a3a,#1a2f6b);color:#fff;padding:70px 20px;text-align:center}
header h1{margin:0;font-size:44px}
header p{opacity:.9}

nav{background:#fff;padding:15px;display:flex;justify-content:center;gap:28px;
box-shadow:0 4px 12px rgba(0,0,0,.05);position:sticky;top:0}
nav a{text-decoration:none;color:#081a3a;font-weight:600}

section{padding:65px 20px;max-width:1100px;margin:auto}
h2{color:#081a3a;margin-bottom:18px}

.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:20px}
.card{background:#fff;padding:22px;border-radius:14px;
box-shadow:0 8px 18px rgba(0,0,0,.06)}

.gallery{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:18px}
.gallery img{width:100%;height:180px;object-fit:cover;border-radius:12px}

button,.btn{
background:#081a3a;color:#fff;border:none;padding:12px 18px;
border-radius:8px;cursor:pointer;font-weight:600}

textarea,input{
width:100%;padding:12px;margin-top:10px;border-radius:8px;border:1px solid #ccc}

.review{background:#fff;padding:14px;border-radius:10px;margin-top:10px;
box-shadow:0 3px 10px rgba(0,0,0,.05)}

.contact-buttons{display:flex;gap:14px;flex-wrap:wrap}
.whatsapp{background:#25D366}
.call{background:#081a3a}

footer{background:#081a3a;color:#fff;text-align:center;padding:28px;margin-top:40px}
</style>
</head>

<body>

<header>
<h1>Kprime Travel Agency</h1>
<p>Luxury hotel bookings • Diani vacations • Seamless travel planning</p>
</header>

<nav>
<a href="#about">About</a>
<a href="#services">Services</a>
<a href="#gallery">Gallery</a>
<a href="#booking">Booking</a>
<a href="#reviews">Reviews</a>
<a href="#contact">Contact</a>
</nav>

<section id="about">
<h2>About Us</h2>
<p>
Kprime Travel Agency specializes in premium hotel bookings and curated travel
experiences across Kenya — especially Diani Beach.  
We help clients secure trusted stays, luxury getaways, and stress-free travel arrangements
with fast response and personalized support.
</p>
</section>

<section id="services">
<h2>Our Services</h2>

<div class="cards">

<div class="card">
<h3>Hotel Bookings</h3>
<p>Verified hotels, apartments, and luxury resorts at competitive rates.</p>
</div>

<div class="card">
<h3>Diani Beach Trips</h3>
<p>Handpicked beach stays and vacation packages in Diani.</p>
</div>

<div class="card">
<h3>Luxury Travel</h3>
<p>Premium stays and exclusive travel experiences for high-end clients.</p>
</div>

<div class="card">
<h3>Corporate Travel</h3>
<p>Reliable accommodation planning for business trips and group travel.</p>
</div>

</div>
</section>

<section id="gallery">
<h2>Gallery (Owner uploads photos)</h2>

<input type="file" id="uploader" multiple hidden>
<button onclick="uploader.click()">Upload Photos</button>

<div class="gallery" id="galleryGrid"></div>
</section>

<section id="booking">
<h2>Request Booking</h2>

<input id="name" placeholder="Your name">
<input id="location" placeholder="Destination / Hotel">
<input id="dates" placeholder="Travel dates">
<button onclick="sendBooking()">Send Booking Request</button>

</section>

<section id="reviews">
<h2>Client Reviews</h2>

<textarea id="reviewText" placeholder="Write your review"></textarea>
<button onclick="addReview()">Submit Review</button>

<div id="reviewsList"></div>
</section>

<section id="contact">
<h2>Contact Us</h2>

<div class="contact-buttons">

<a class="btn whatsapp"
href="https://wa.me/254723718279?text=Hello%20Kprime%20Travel%20Agency"
target="_blank">WhatsApp</a>

<a class="btn call"
href="tel:+254723718279">Call</a>

<a class="btn call"
href="mailto:Kprime.travel.ke@gmail.com">Email</a>

</div>

<p style="margin-top:20px;">
Phone: +254 723 718279<br>
Email: Kprime.travel.ke@gmail.com
</p>

</section>

<footer>
© 2026 Kprime Travel Agency — Premium Travel Services
</footer>

<script>

/* gallery upload */
const uploader=document.getElementById("uploader");
const gallery=document.getElementById("galleryGrid");

uploader.addEventListener("change",()=>{
[...uploader.files].forEach(file=>{
const reader=new FileReader();
reader.onload=e=>{
const img=document.createElement("img");
img.src=e.target.result;
gallery.appendChild(img);
};
reader.readAsDataURL(file);
});
});

/* reviews */
function addReview(){
const text=document.getElementById("reviewText").value.trim();
if(!text) return;
const div=document.createElement("div");
div.className="review";
div.textContent=text;
document.getElementById("reviewsList").prepend(div);
document.getElementById("reviewText").value="";
}

/* booking -> whatsapp */
function sendBooking(){
const name=document.getElementById("name").value;
const loc=document.getElementById("location").value;
const dates=document.getElementById("dates").value;

const msg=`Hello Kprime Travel Agency,%0AName: ${name}%0ADestination: ${loc}%0ADates: ${dates}`;
window.open(`https://wa.me/254723718279?text=${msg}`,'_blank');
}

</script>

</body>
</html>
