<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bendo Uyay'dlalela | Official Music Hub</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons for Socials & Buttons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Modern Bold Typography -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&family=Orbitron:wght@600;800;900&display=swap" rel="stylesheet">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'neon-pink': '#ff007f',
                        'neon-cyan': '#00f3ff',
                        'neon-yellow': '#ffe600',
                        'neon-lime': '#39ff14',
                        'dark-bg': '#07060c',
                        'card-bg': '#12101e'
                    },
                    fontFamily: {
                        orbitron: ['Orbitron', 'sans-serif'],
                        montserrat: ['Montserrat', 'sans-serif'],
                    },
                    boxShadow: {
                        'pink-glow': '0 0 20px rgba(255, 0, 127, 0.6)',
                        'cyan-glow': '0 0 20px rgba(0, 243, 255, 0.6)',
                        'yellow-glow': '0 0 20px rgba(255, 230, 0, 0.6)',
                        'lime-glow': '0 0 20px rgba(57, 255, 20, 0.6)',
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #07060c;
            color: #ffffff;
            overflow-x: hidden;
        }

        /* Pulsing Radial Background Gradient */
        .glow-bg {
            background: radial-gradient(circle at 50% 15%, rgba(255, 0, 127, 0.18), rgba(0, 243, 255, 0.12), transparent 75%);
        }

        /* Glassmorphism Card Style */
        .neon-card {
            background: rgba(18, 16, 30, 0.85);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .neon-card:hover {
            border-color: #00f3ff;
            box-shadow: 0 0 20px rgba(0, 243, 255, 0.4);
            transform: translateY(-2px);
        }

        /* Neon Glow Texts */
        .neon-text-pink {
            text-shadow: 0 0 10px rgba(255, 0, 127, 0.8), 0 0 20px rgba(255, 0, 127, 0.4);
        }

        .neon-text-cyan {
            text-shadow: 0 0 10px rgba(0, 243, 255, 0.8), 0 0 20px rgba(0, 243, 255, 0.4);
        }

        .neon-text-yellow {
            text-shadow: 0 0 10px rgba(255, 230, 0, 0.8), 0 0 20px rgba(255, 230, 0, 0.4);
        }

        /* Dynamic Navigation Tab Active State */
        .tab-btn.active {
            color: #00f3ff;
            border-bottom: 3px solid #00f3ff;
            text-shadow: 0 0 12px rgba(0, 243, 255, 0.9);
        }
    </style>
</head>
<body class="glow-bg min-h-screen flex flex-col justify-between">

    <!-- Top Navigation Header -->
    <header class="sticky top-0 z-50 bg-[#07060c]/90 backdrop-blur-md border-b border-gray-800/80">
        <div class="max-w-5xl mx-auto px-4 py-4 flex flex-col sm:flex-row justify-between items-center gap-4">
            
            <!-- Artist Brand Logo -->
            <a href="#" class="font-orbitron font-black text-xl sm:text-2xl tracking-wider text-transparent bg-clip-text bg-gradient-to-r from-neon-pink via-neon-cyan to-neon-yellow">
                BENDO <span class="text-white font-semibold text-base sm:text-lg">UYAY'DLALELA</span>
            </a>

            <!-- Navigation Bar Tabs -->
            <nav class="flex items-center space-x-4 sm:space-x-8 font-orbitron text-xs sm:text-sm font-bold">
                <button onclick="switchTab('music')" id="tab-music" class="tab-btn active py-2 text-gray-300 hover:text-neon-cyan transition flex items-center gap-2">
                    <i class="fa-solid fa-compact-disc text-neon-pink"></i> MUSIC
                </button>
                <button onclick="switchTab('photos')" id="tab-photos" class="tab-btn py-2 text-gray-300 hover:text-neon-cyan transition flex items-center gap-2">
                    <i class="fa-solid fa-camera text-neon-cyan"></i> PHOTOS
                </button>
                <button onclick="switchTab('booking')" id="tab-booking" class="tab-btn py-2 text-gray-300 hover:text-neon-cyan transition flex items-center gap-2">
                    <i class="fa-solid fa-paper-plane text-neon-yellow"></i> BOOKINGS & CONNECT
                </button>
            </nav>
        </div>
    </header>

    <!-- Main Content Container -->
    <main class="max-w-4xl mx-auto px-4 py-8 flex-grow w-full">

        <!-- ================= TAB 1: MUSIC & SMARTLINKS ================= -->
        <section id="section-music" class="space-y-8 animate-fadeIn">
            
            <!-- Hero Title & Subtitle -->
            <div class="text-center space-y-2">
                <span class="inline-block bg-neon-pink/20 border border-neon-pink text-neon-pink text-xs font-orbitron font-black px-4 py-1 rounded-full tracking-widest shadow-pink-glow uppercase">
                    ⚡ GQOM PRODUCER & ARTIST
                </span>
                <h1 class="text-3xl sm:text-5xl font-black font-orbitron text-white">
                    OFFICIAL <span class="text-neon-cyan neon-text-cyan">MUSIC HUB</span>
                </h1>
                <p class="text-gray-400 text-xs sm:text-sm max-w-md mx-auto">
                    Listen to latest tracks, stream releases, and pre-save upcoming bangers directly on Ditto.
                </p>
            </div>

            <!-- Pre-Save Single Promo Banner -->
            <div class="neon-card p-6 rounded-2xl border-l-4 border-l-neon-yellow flex flex-col sm:flex-row justify-between items-center gap-4 shadow-yellow-glow/20">
                <div class="text-center sm:text-left">
                    <span class="text-neon-yellow text-xs font-orbitron font-bold uppercase tracking-wider flex items-center justify-center sm:justify-start gap-1">
                        <i class="fa-solid fa-fire text-neon-pink"></i> Upcoming Release
                    </span>
                    <h2 class="text-2xl font-orbitron font-black text-white mt-1">"FAST LANE"</h2>
                    <p class="text-xs text-gray-300">Be the first to listen when it drops.</p>
                </div>
                <a href="https://ditto.fm/fast-lane-bendo-uyay-dlalela" target="_blank" class="w-full sm:w-auto bg-gradient-to-r from-neon-pink to-purple-600 hover:from-pink-600 hover:to-purple-700 text-white font-orbitron font-bold py-3 px-6 rounded-xl shadow-pink-glow transition duration-300 text-center text-sm flex items-center justify-center gap-2">
                    <i class="fa-solid fa-bolt"></i> 🔥 PRE-SAVE UPCOMING SINGLE
                </a>
            </div>

            <!-- Embedded Ditto Release Player -->
            <div class="neon-card p-4 sm:p-6 rounded-2xl space-y-3">
                <div class="flex justify-between items-center border-b border-gray-800 pb-3">
                    <h3 class="font-orbitron font-bold text-white text-base sm:text-lg flex items-center gap-2">
                        <i class="fa-solid fa-circle-play text-neon-cyan"></i> LATEST RELEASE: "STILL STANDING"
                    </h3>
                    <span class="text-xs text-neon-cyan font-orbitron hidden sm:inline-block">DITTO SMARTLINK</span>
                </div>
                
                <!-- Live Embedded SmartLink Player -->
                <div class="w-full overflow-hidden rounded-xl border border-neon-cyan/30 shadow-cyan-glow">
                    <iframe src="https://ditto.fm/still-standing-bendo-uyay-dlalela" width="100%" height="480" style="border-radius:12px; background:#111;"></iframe>
                </div>
            </div>

            <!-- Social Media Quick Bar -->
            <div class="neon-card p-5 rounded-2xl space-y-4 text-center">
                <h4 class="font-orbitron font-bold text-sm text-neon-yellow uppercase tracking-wider">
                    CONNECT ACROSS PLATFORMS
                </h4>
                <div class="flex flex-wrap justify-center gap-3 sm:gap-4 text-xs sm:text-sm font-bold">
                    <a href="https://www.instagram.com/bendo_uyay_dlalela/" target="_blank" class="bg-gradient-to-r from-purple-600 to-pink-500 hover:opacity-90 text-white px-4 py-2.5 rounded-xl transition flex items-center gap-2">
                        <i class="fa-brands fa-instagram text-base"></i> Instagram
                    </a>
                    <a href="https://www.facebook.com/profile.php?id=100076414345954" target="_blank" class="bg-blue-600 hover:bg-blue-700 text-white px-4 py-2.5 rounded-xl transition flex items-center gap-2">
                        <i class="fa-brands fa-facebook-f text-base"></i> Facebook
                    </a>
                    <a href="https://www.tiktok.com/@bendo_uyaydlalela" target="_blank" class="bg-black border border-neon-cyan hover:border-neon-pink text-white px-4 py-2.5 rounded-xl transition flex items-center gap-2 shadow-cyan-glow/30">
                        <i class="fa-brands fa-tiktok text-base text-neon-cyan"></i> TikTok
                    </a>
                    <a href="https://www.youtube.com/channel/UCT2ukkZ4S2lLJWJG0-gnWHA" target="_blank" class="bg-red-600 hover:bg-red-700 text-white px-4 py-2.5 rounded-xl transition flex items-center gap-2">
                        <i class="fa-brands fa-youtube text-base"></i> YouTube
                    </a>
                </div>
            </div>

        </section>

        <!-- ================= TAB 2: PHOTO GALLERY ================= -->
        <section id="section-photos" class="hidden space-y-6 animate-fadeIn">
            
            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center border-b border-gray-800 pb-4 gap-2">
                <div>
                    <h2 class="text-2xl sm:text-3xl font-orbitron font-black text-neon-cyan neon-text-cyan">
                        GALLERY & STAGE SHOTS
                    </h2>
                    <p class="text-gray-400 text-xs">Live performances, studio moments, and visuals.</p>
                </div>
                <span class="text-xs font-orbitron text-neon-lime bg-lime-500/10 border border-neon-lime px-3 py-1 rounded-full">
                    <i class="fa-solid fa-expand"></i> Click photo to view full size
                </span>
            </div>

            <!-- Responsive Image Grid -->
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
                
                <!-- Photo 1 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?auto=format&fit=crop&w=800&q=80', 'Mainstage Performance')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?auto=format&fit=crop&w=800&q=80" alt="Live Gig" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-cyan font-orbitron text-xs font-bold"><i class="fa-solid fa-bolt"></i> Live Stage Session</p>
                    </div>
                </div>

                <!-- Photo 2 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?auto=format&fit=crop&w=800&q=80', 'Studio Beat Production')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?auto=format&fit=crop&w=800&q=80" alt="Studio" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-pink font-orbitron text-xs font-bold"><i class="fa-solid fa-sliders"></i> Studio Gqom Sessions</p>
                    </div>
                </div>

                <!-- Photo 3 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1470225620780-dba8ba36b745?auto=format&fit=crop&w=800&q=80', 'Club Event Party')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1470225620780-dba8ba36b745?auto=format&fit=crop&w=800&q=80" alt="Club Event" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-yellow font-orbitron text-xs font-bold"><i class="fa-solid fa-music"></i> Nightclub Energy</p>
                    </div>
                </div>

                <!-- Photo 4 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1514525253161-7a46d19cd819?auto=format&fit=crop&w=800&q=80', 'Festival Vibes')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1514525253161-7a46d19cd819?auto=format&fit=crop&w=800&q=80" alt="Festival" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-lime font-orbitron text-xs font-bold"><i class="fa-solid fa-users"></i> Crowd Reaction</p>
                    </div>
                </div>

                <!-- Photo 5 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1511671782779-c97d3d27a1d4?auto=format&fit=crop&w=800&q=80', 'Single Release Artwork')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1511671782779-c97d3d27a1d4?auto=format&fit=crop&w=800&q=80" alt="Cover Art" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-pink font-orbitron text-xs font-bold"><i class="fa-solid fa-record-vinyl"></i> Cover Art Concept</p>
                    </div>
                </div>

                <!-- Photo 6 -->
                <div onclick="openLightbox('https://images.unsplash.com/photo-1501386761578-eac5c94b800a?auto=format&fit=crop&w=800&q=80', 'Tour Life')" class="neon-card rounded-xl overflow-hidden cursor-pointer group relative">
                    <img src="https://images.unsplash.com/photo-1501386761578-eac5c94b800a?auto=format&fit=crop&w=800&q=80" alt="Tour" class="w-full h-56 object-cover group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent opacity-0 group-hover:opacity-100 transition duration-300 flex items-end p-3">
                        <p class="text-neon-cyan font-orbitron text-xs font-bold"><i class="fa-solid fa-plane"></i> Tour Highlights</p>
                    </div>
                </div>

            </div>
        </section>

        <!-- ================= TAB 3: BOOKINGS & CONNECT ================= -->
        <section id="section-booking" class="hidden space-y-8 animate-fadeIn">
            
            <div class="neon-card p-6 sm:p-8 rounded-2xl border-t-4 border-t-neon-lime">
                <div class="text-center space-y-2 mb-8">
                    <h2 class="text-2xl sm:text-3xl font-orbitron font-black text-white">
                        BOOKINGS & <span class="text-neon-lime neon-text-yellow">ENQUIRIES</span>
                    </h2>
                    <p class="text-gray-300 text-xs sm:text-sm">
                        Available for festival slots, club performances, features, and custom beat production.
                    </p>
                </div>

                <!-- Instant WhatsApp Direct Button -->
                <div class="bg-gradient-to-r from-emerald-600 to-teal-600 p-6 rounded-xl text-center space-y-3 mb-8 shadow-lime-glow/20">
                    <i class="fa-brands fa-whatsapp text-4xl text-white"></i>
                    <h3 class="text-lg font-orbitron font-bold text-white">INSTANT BOOKING CHAT</h3>
                    <p class="text-xs text-emerald-100">Click below to chat directly on WhatsApp for performance inquiries and rates.</p>
                    <a href="https://wa.me/27123456789?text=Hi%20Bendo%20Uyay'dlalela,%20I'm%20inquiring%20about%20a%20booking%20or%20collaboration." target="_blank" class="inline-block bg-white text-emerald-900 font-orbitron font-black px-8 py-3 rounded-xl shadow-md hover:bg-emerald-100 transition text-xs sm:text-sm">
                        <i class="fa-brands fa-whatsapp text-emerald-600"></i> CHAT ON WHATSAPP NOW
                    </a>
                </div>

                <!-- Quick Booking Message Form -->
                <form onsubmit="event.preventDefault(); triggerFormMsg();" class="space-y-4">
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div>
                            <label class="block text-xs font-orbitron text-gray-300 mb-1">Your Name / Promoter</label>
                            <input type="text" required placeholder="e.g. John Khumalo" class="w-full bg-black/70 border border-gray-700 focus:border-neon-lime rounded-xl p-3 text-white text-sm outline-none">
                        </div>
                        <div>
                            <label class="block text-xs font-orbitron text-gray-300 mb-1">Email / Phone</label>
                            <input type="text" required placeholder="contact@example.com" class="w-full bg-black/70 border border-gray-700 focus:border-neon-lime rounded-xl p-3 text-white text-sm outline-none">
                        </div>
                    </div>

                    <div>
                        <label class="block text-xs font-orbitron text-gray-300 mb-1">Enquiry Type</label>
                        <select class="w-full bg-black/70 border border-gray-700 focus:border-neon-lime rounded-xl p-3 text-white text-sm outline-none">
                            <option>Club Gig / Live Performance</option>
                            <option>Festival Stage Booking</option>
                            <option>Feature / Song Collaboration</option>
                            <option>Beat Production Enquiry</option>
                        </select>
                    </div>

                    <div>
                        <label class="block text-xs font-orbitron text-gray-300 mb-1">Message / Event Details</label>
                        <textarea rows="4" required placeholder="Include date, location, and venue details..." class="w-full bg-black/70 border border-gray-700 focus:border-neon-lime rounded-xl p-3 text-white text-sm outline-none"></textarea>
                    </div>

                    <button type="submit" class="w-full bg-neon-lime text-black font-orbitron font-black py-3.5 rounded-xl hover:bg-lime-400 transition shadow-lime-glow text-sm">
                        SEND BOOKING REQUEST
                    </button>
                </form>

                <div id="booking-msg" class="hidden mt-4 p-4 rounded-xl bg-emerald-900/60 border border-emerald-500 text-emerald-200 text-center text-xs font-orbitron">
                    <i class="fa-solid fa-circle-check"></i> Request received! Bendo Uyay'dlalela's team will get back to you shortly.
                </div>
            </div>

        </section>

    </main>

    <!-- Lightbox Modal for Photo Gallery -->
    <div id="lightbox" class="fixed inset-0 bg-black/95 z-50 hidden flex-col justify-center items-center p-4">
        <button onclick="closeLightbox()" class="absolute top-6 right-6 text-white text-3xl hover:text-neon-pink">
            <i class="fa-solid fa-xmark"></i>
        </button>
        <img id="lightbox-img" src="" alt="Enlarged Visual" class="max-w-full max-h-[80vh] rounded-xl border-2 border-neon-cyan shadow-cyan-glow object-contain">
        <p id="lightbox-caption" class="text-neon-cyan font-orbitron mt-4 font-bold text-center text-sm"></p>
    </div>

    <!-- Website Footer -->
    <footer class="border-t border-gray-800 bg-black/90 py-8 px-4 mt-8">
        <div class="max-w-4xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-4 text-center sm:text-left">
            <div>
                <p class="font-orbitron font-bold text-white text-sm">BENDO UYAY'DLALELA</p>
                <p class="text-xs text-gray-400">Official Gqom Artist & Producer Portal</p>
            </div>

            <!-- Social Links in Footer -->
            <div class="flex items-center space-x-5 text-xl">
                <a href="https://www.instagram.com/bendo_uyay_dlalela/" target="_blank" class="text-gray-400 hover:text-neon-pink transition">
                    <i class="fa-brands fa-instagram"></i>
                </a>
                <a href="https://www.facebook.com/profile.php?id=100076414345954" target="_blank" class="text-gray-400 hover:text-blue-500 transition">
                    <i class="fa-brands fa-facebook"></i>
                </a>
                <a href="https://www.tiktok.com/@bendo_uyaydlalela" target="_blank" class="text-gray-400 hover:text-neon-cyan transition">
                    <i class="fa-brands fa-tiktok"></i>
                </a>
                <a href="https://www.youtube.com/channel/UCT2ukkZ4S2lLJWJG0-gnWHA" target="_blank" class="text-gray-400 hover:text-red-500 transition">
                    <i class="fa-brands fa-youtube"></i>
                </a>
            </div>

            <p class="text-xs text-gray-500 font-montserrat">
                &copy; 2026 Bendo Uyay'dlalela.
            </p>
        </div>
    </footer>

    <!-- Interactive Navigation & Gallery Scripts -->
    <script>
        // Tab Switch Logic
        function switchTab(tabName) {
            document.getElementById('section-music').classList.add('hidden');
            document.getElementById('section-photos').classList.add('hidden');
            document.getElementById('section-booking').classList.add('hidden');

            document.getElementById('tab-music').classList.remove('active');
            document.getElementById('tab-photos').classList.remove('active');
            document.getElementById('tab-booking').classList.remove('active');

            document.getElementById('section-' + tabName).classList.remove('hidden');
            document.getElementById('tab-' + tabName).classList.add('active');
        }

        // Lightbox Modal Logic
        function openLightbox(imgSrc, caption) {
            document.getElementById('lightbox-img').src = imgSrc;
            document.getElementById('lightbox-caption').innerText = caption;
            document.getElementById('lightbox').classList.remove('hidden');
            document.getElementById('lightbox').classList.add('flex');
        }

        function closeLightbox() {
            document.getElementById('lightbox').classList.add('hidden');
            document.getElementById('lightbox').classList.remove('flex');
        }

        // Form Notification Action
        function triggerFormMsg() {
            const msg = document.getElementById('booking-msg');
            msg.classList.remove('hidden');
            setTimeout(() => {
                msg.classList.add('hidden');
            }, 4000);
        }
    </script>
</body>
</html>
