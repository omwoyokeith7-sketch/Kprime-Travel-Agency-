<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KPrime Travel Agency | Global Luxury Portal</title>
    
    <!-- Professional Icons & Fonts -->
    <link href="https://cdnjs.cloudflare.com" rel="stylesheet">
    <link href="https://fonts.googleapis.com" rel="stylesheet">
    
    <style>
        :root {
            --primary: #0a192f;
            --accent: #ffb400;
            --glass: rgba(255, 255, 255, 0.9);
            --card-bg: #ffffff;
            --text-main: #1a1a1a;
            --shadow: 0 12px 40px rgba(0,0,0,0.08);
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Plus Jakarta Sans', sans-serif; scroll-behavior: smooth; }
        body { background: #f4f7fa; color: var(--text-main); line-height: 1.6; }

        /* MULTI-CHANNEL NAVIGATION */
        nav {
            background: var(--glass); backdrop-filter: blur(15px);
            padding: 15px 6%; display: flex; justify-content: space-between; align-items: center;
            position: sticky; top: 0; z-index: 1000; border-bottom: 1px solid rgba(0,0,0,0.05);
        }
        .logo { font-size: 24px; font-weight: 800; letter-spacing: -1px; color: var(--primary); }
        .logo span { color: var(--accent); }

        .nav-links { display: flex; gap: 25px; align-items: center; }
        .nav-links a { text-decoration: none; color: var(--primary); font-weight: 600; font-size: 14px; transition: 0.3s; }
        .nav-links a:hover { color: var(--accent); }

        /* BENTO GRID SYSTEM */
        .main-container {
            max-width: 1300px; margin: 30px auto; padding: 0 20px;
            display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px;
        }

        .bento-card {
            background: var(--card-bg); border-radius: 24px; padding: 25px;
            box-shadow: var(--shadow); border: 1px solid rgba(255,255,255,0.8);
            transition: transform 0.3s ease;
        }
        .bento-card:hover { transform: translateY(-5px); }

        /* HERO / SEARCH BOX (Large) */
        .hero-card { 
            grid-column: span 3; background: linear-gradient(135deg, #081a3a 0%, #1a2f6b 100%);
            color: white; display: flex; flex-direction: column; justify-content: center;
        }
        .hero-card h1 { font-size: 42px; margin-bottom: 15px; }
        
        .search-engine {
            background: white; border-radius: 16px; padding: 10px;
            display: grid; grid-template-columns: 2fr 1fr 1fr auto; gap: 10px; margin-top: 20px;
        }
        .search-engine input { border: none; padding: 12px; outline: none; font-size: 14px; border-right: 1px solid #eee; }
        .btn-search { background: var(--accent); border: none; border-radius: 12px; padding: 0 30px; font-weight: 800; cursor: pointer; transition: 0.2s; }
        .btn-search:hover { background: #e5a200; transform: scale(1.05); }

        /* ICON CARDS */
        .icon-card { text-align: center; }
        .icon-card i { font-size: 32px; color: var(--accent); margin-bottom: 15px; }
        .icon-card h3 { font-size: 18px; margin-bottom: 8px; }
        .icon-card p { font-size: 13px; color: #666; }

        /* TIKTOK / SOCIAL PROOF CARD */
        .social-card { background: #000; color: white; grid-row: span 1; }
        .social-card i { color: #ff0050; font-size: 40px; margin-bottom: 20px; }
        .btn-tiktok { background: #fff; color: #000; border: none; padding: 10px 20px; border-radius: 50px; font-weight: 800; width: 100%; margin-top: 15px; cursor: pointer; }

        /* GALLERY & REVIEWS (Auto-Populating) */
        .full-width { grid-column: span 4; }
        .gallery-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); gap: 15px; margin-top: 20px; }
        .gallery-grid img { width: 100%; height: 150px; object-fit: cover; border-radius: 15px; }

        /* FLOATING MULTI-CONTACT HUB */
        .contact-hub { position: fixed; bottom: 30px; right: 30px; z-index: 9999; }
        .hub-btn { 
            width: 65px; height: 65px; border-radius: 50%; background: var(--primary); 
            color: white; border: none; font-size: 24px; cursor: pointer; box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        .hub-options { 
            position: absolute; bottom: 80px; right: 0; display: none; flex-direction: column; gap: 12px;
        }
        .hub-options a { 
            padding: 12px 25px; border-radius: 50px; text-decoration: none; color: white; font-weight: 600;
            display: flex; align-items: center; gap: 10px; white-space: nowrap; transition: 0.3s;
        }

        /* MOBILE FIXES */
        @media (max-width: 900px) {
            .main-container { grid-template-columns: 1fr; }
            .hero-card, .full-width { grid-column: span 1; }
            .search-engine { grid-template-columns: 1fr; }
            .search-engine input { border-right: none; border-bottom: 1px solid #eee; }
        }
    </style>
</head>
<body>

<nav>
    <div class="logo">KPRIME<span>TRAVEL</span></div>
    <div class="nav-links">
        <a href="#services">Services</a>
        <a href="#gallery">Gallery</a>
        <a href="mailto:Kprime.travel.ke@gmail.com"><i class="fas fa-envelope"></i> Email</a>
        <a href="tel:+254723718279"><i class="fas fa-phone"></i> Call</a>
    </div>
</nav>

<div class="main-container">
    
    <!-- Automated Booking Engine (Bento Main) -->
    <div class="bento-card hero-card">
        <h1>Bespoke Luxury Stays</h1>
        <p>Your portal to exclusive Diani villas and global hotel reservations.</p>
        
        <div class="search-engine">
            <input type="text" id="dest" placeholder="Where are we going?">
            <input type="text" id="dates" placeholder="Travel Dates" onfocus="(this.type='date')">
            <input type="number" id="guests" placeholder="Guests">
            <button class="btn-search" onclick="sendAutomatedRequest()">SEARCH</button>
        </div>
    </div>

    <!-- TikTok Branding Card -->
    <div class="bento-card social-card">
        <i class="fab fa-tiktok"></i>
        <h3>Follow Our Tours</h3>
        <p>Real-time travel vlogs from the Maasai Mara to the Coast.</p>
        <button class="btn-tiktok" onclick="window.open('https://www.tiktok.com', '_blank')">Follow @KPrime</button>
    </div>

    <!-- Service Icons -->
    <div class="bento-card icon-card">
        <i class="fas fa-hotel"></i>
        <h3>Elite Stays</h3>
        <p>Hand-picked apartments & 5-star resorts.</p>
    </div>

    <div class="bento-card icon-card">
        <i class="fas fa-shuttle-van"></i>
        <h3>VIP Transfers</h3>
        <p>Automated airport pickup arrangements.</p>
    </div>

    <div class="bento-card icon-card">
        <i class="fas fa-umbrella-beach"></i>
        <h3>Diani Expert</h3>
        <p>The #1 agency for Diani Beach vacations.</p>
    </div>

    <!-- Review Section -->
    <div class="bento-card">
        <h3>Client Reviews</h3>
        <div id="reviewsList" style="max-height: 150px; overflow-y: auto; margin-bottom: 10px;">
            <p style="font-size: 13px; font-style: italic;">"Best experience in Diani ever!" - Sarah M.</p>
        </div>
        <input type="text" id="revInput" placeholder="Add a review..." style="width:100%; padding:8px; border-radius:8px; border:1px solid #ddd;">
        <button onclick="addReview()" style="width:100%; margin-top:10px; padding:8px; border:none; background:var(--primary); color:white; border-radius:8px; cursor:pointer;">Post</button>
    </div>

    <!-- Media Gallery -->
    <div class="bento-card full-width" id="gallery">
        <div style="display:flex; justify-content:space-between; align-items:center;">
            <h3>Exclusive Gallery</h3>
            <input type="file" id="upload" hidden multiple>
            <button class="btn-search" style="padding:8px 15px;" onclick="document.getElementById('upload').click()">+ Add Photos</button>
        </div>
        <div class="gallery-grid" id="galleryGrid">
            <!-- Sample Image -->
            <img src="https://images.unsplash.com" alt="Diani">
        </div>
    </div>
</div>

<!-- FLOATING COMMUNICATION HUB -->
<div class="contact-hub">
    <div class="hub-options" id="hub">
        <a href="https://wa.me" style="background:#25D366;"><i class="fab fa-whatsapp"></i> WhatsApp</a>
        <a href="tel:+254723718279" style="background:var(--primary);"><i class="fas fa-phone"></i> Call Agency</a>
        <a href="mailto:Kprime.travel.ke@gmail.com" style="background:#ea4335;"><i class="fas fa-envelope"></i> Email Support</a>
        <a href="https://www.tiktok.com" style="background:#000;"><i class="fab fa-tiktok"></i> TikTok</a>
    </div>
    <button class="hub-btn" onclick="toggleHub()">
        <i class="fas fa-comments"></i>
    </button>
</div>

<script>
    // Automated Communication Logic
    function sendAutomatedRequest() {
        const dest = document.getElementById('dest').value;
        const date = document.getElementById('dates').value;
        const guests = document.getElementById('guests').value;

        if(!dest) { alert("Please enter a destination!"); return; }

        const message = `Hello KPrime Travel! I am using your automated portal to request a booking:%0A%0A📍 Destination: ${dest}%0A📅 Dates: ${date}%0A👥 Guests: ${guests}%0A%0APlease let me know available luxury options.`;
        window.open(`https://wa.me/254723718279?text=${message}`, '_blank');
    }

    // Hub Toggle
    function toggleHub() {
        const hub = document.getElementById('hub');
        hub.style.display = hub.style.display === 'flex' ? 'none' : 'flex';
    }

    // Review Logic
    function addReview() {
        const input = document.getElementById('revInput');
        if(!input.value) return;
        const div = document.createElement('p');
        div.style.fontSize = "13px";
        div.style.marginBottom = "5px";
        div.innerHTML = `⭐ <b>You:</b> ${input.value}`;
        document.getElementById('reviewsList').prepend(div);
        input.value = "";
    }

    // Gallery Logic
    document.getElementById('upload').addEventListener('change', function() {
        [...this.files].forEach(file => {
            const reader = new FileReader();
            reader.onload = e => {
                const img = document.createElement('img');
                img.src = e.target.result;
                document.getElementById('galleryGrid').prepend(img);
            }
            reader.readAsDataURL(file);
        });
    });
</script>

</body>
</html>
