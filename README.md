<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KPrime Travel Agency | Luxury Kenya Safaris</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com" rel="stylesheet">
    <style>
        html { scroll-behavior: smooth; }
        .hero-bg {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), 
                        url('https://images.unsplash.com');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-white/90 backdrop-blur-md shadow-sm">
        <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold tracking-tighter text-blue-900">KPRIME<span class="text-amber-600">TRAVEL</span></h1>
            <div class="hidden md:flex space-x-8 font-medium">
                <a href="#" class="hover:text-amber-600 transition">Home</a>
                <a href="#services" class="hover:text-amber-600 transition">Services</a>
                <a href="#booking" class="hover:text-amber-600 transition">Booking</a>
                <a href="#contact" class="hover:text-amber-600 transition">Contact</a>
            </div>
            <a href="https://wa.me" class="bg-green-500 text-white px-5 py-2 rounded-full flex items-center hover:bg-green-600 transition">
                <i class="fab fa-whatsapp mr-2"></i> WhatsApp
            </a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="hero-bg h-screen flex items-center justify-center text-center text-white px-4">
        <div class="max-w-3xl">
            <h2 class="text-5xl md:text-7xl font-bold mb-6">Luxury Travel Experiences</h2>
            <p class="text-xl md:text-2xl mb-8 font-light">Your gateway to exclusive hotel bookings, unforgettable tours, and tailored holiday packages across Kenya.</p>
            <div class="flex flex-col md:flex-row gap-4 justify-center">
                <a href="#booking" class="bg-amber-600 hover:bg-amber-700 text-white px-8 py-4 rounded-lg text-lg font-semibold transition">Book Now</a>
                <a href="mailto:Kprime.travel.ke@gmail.com" class="bg-white/20 hover:bg-white/30 backdrop-blur-md text-white border border-white px-8 py-4 rounded-lg text-lg font-semibold transition">Email Us</a>
            </div>
        </div>
    </header>

    <!-- Services Section -->
    <section id="services" class="py-20 max-w-7xl mx-auto px-4">
        <div class="text-center mb-16">
            <h2 class="text-4xl font-bold text-blue-900 mb-4">Our Services</h2>
            <div class="w-20 h-1 bg-amber-600 mx-auto"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
            <!-- Hotel Bookings -->
            <div class="bg-white p-8 rounded-xl shadow-lg border-b-4 border-amber-600 hover:-translate-y-2 transition">
                <div class="text-amber-600 text-4xl mb-4"><i class="fas fa-hotel"></i></div>
                <h3 class="text-xl font-bold mb-3">Hotel Bookings</h3>
                <p class="text-gray-600">Exclusive hotel deals in Diani and across Kenya for every budget.</p>
            </div>

            <!-- Holiday Packages -->
            <div class="bg-white p-8 rounded-xl shadow-lg border-b-4 border-amber-600 hover:-translate-y-2 transition">
                <div class="text-amber-600 text-4xl mb-4"><i class="fas fa-map-marked-alt"></i></div>
                <h3 class="text-xl font-bold mb-3">Holiday Packages</h3>
                <p class="text-gray-600">Custom packages for couples, families, and groups with unforgettable experiences.</p>
            </div>

            <!-- Transfers -->
            <div class="bg-white p-8 rounded-xl shadow-lg border-b-4 border-amber-600 hover:-translate-y-2 transition">
                <div class="text-amber-600 text-4xl mb-4"><i class="fas fa-shuttle-van"></i></div>
                <h3 class="text-xl font-bold mb-3">Transfers</h3>
                <p class="text-gray-600">Reliable airport pickups and local transport to make your trip seamless.</p>
            </div>

            <!-- Tours & Safaris -->
            <div class="bg-white p-8 rounded-xl shadow-lg border-b-4 border-amber-600 hover:-translate-y-2 transition">
                <div class="text-amber-600 text-4xl mb-4"><i class="fas fa-binoculars"></i></div>
                <h3 class="text-xl font-bold mb-3">Tours & Safaris</h3>
                <p class="text-gray-600">Curated safaris and tours to explore Kenya’s top destinations and hidden gems.</p>
            </div>
        </div>
    </section>

    <!-- Booking Section -->
    <section id="booking" class="py-20 bg-blue-900 text-white">
        <div class="max-w-4xl mx-auto px-4 text-center">
            <h2 class="text-4xl font-bold mb-8">Request a Booking</h2>
            <form action="mailto:Kprime.travel.ke@gmail.com" method="post" enctype="text/plain" class="space-y-4">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <input type="text" placeholder="Your Name" class="w-full p-4 rounded-lg text-gray-800 focus:ring-2 focus:ring-amber-600 outline-none">
                    <input type="email" placeholder="Email Address" class="w-full p-4 rounded-lg text-gray-800 focus:ring-2 focus:ring-amber-600 outline-none">
                </div>
                <textarea name="requests" placeholder="Special Requests (Destination, Number of People, Dates...)" rows="4" class="w-full p-4 rounded-lg text-gray-800 focus:ring-2 focus:ring-amber-600 outline-none"></textarea>
                <button type="submit" class="w-full bg-amber-600 hover:bg-amber-700 text-white font-bold py-4 rounded-lg transition text-lg">
                    Submit Booking Request
                </button>
            </form>
        </div>
    </section>

    <!-- Contact Section -->
    <footer id="contact" class="bg-gray-900 text-white py-16">
        <div class="max-w-7xl mx-auto px-4 grid grid-cols-1 md:grid-cols-3 gap-12 border-b border-gray-800 pb-12">
            <div>
                <h3 class="text-2xl font-bold mb-6 text-amber-600">KPrime Travel Agency</h3>
                <p class="text-gray-400">Making your Kenyan dream holiday a reality with personalized service and local expertise.</p>
            </div>
            <div>
                <h4 class="text-lg font-semibold mb-6">Contact Info</h4>
                <ul class="space-y-4 text-gray-400">
                    <li><i class="fas fa-phone mr-3 text-amber-600"></i> +254 723 718279</li>
                    <li><i class="fas fa-envelope mr-3 text-amber-600"></i> Kprime.travel.ke@gmail.com</li>
                    <li><i class="fas fa-map-marker-alt mr-3 text-amber-600"></i> Kenya</li>
                </ul>
            </div>
            <div>
                <h4 class="text-lg font-semibold mb-6">Quick Links</h4>
                <div class="flex space-x-4">
                    <a href="https://wa.me" class="w-12 h-12 bg-green-600 flex items-center justify-center rounded-full hover:bg-green-700 transition">
                        <i class="fab fa-whatsapp text-xl"></i>
                    </a>
                    <a href="mailto:Kprime.travel.ke@gmail.com" class="w-12 h-12 bg-blue-600 flex items-center justify-center rounded-full hover:bg-blue-700 transition">
                        <i class="fas fa-envelope text-xl"></i>
                    </a>
                </div>
            </div>
        </div>
        <div class="text-center pt-8 text-gray-500 text-sm">
            &copy; 2026 KPrime Travel Agency. All Rights Reserved.
        </div>
    </footer>

</body>
</html>
