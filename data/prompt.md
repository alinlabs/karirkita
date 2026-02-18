PROJECT NAME:
Purwawisata

DOMAIN:
www.purwawisata.id

TAGLINE:
Jelajahi Keindahan Nusantara

PROJECT TYPE:
Tourism Directory + Hotel Booking + Travel Agency Marketplace + Ticket Platform

STACK:
React + TypeScript + Vite + Tailwind CSS

====================================================

🎯 KONSEP UTAMA PLATFORM

Purwawisata adalah platform pariwisata modern (All-in-One Travel Platform) untuk:

1. Eksplorasi Destinasi (Alam, Budaya, Kuliner)
2. Pemesanan Hotel & Penginapan
3. **Pencarian Agensi Travel Lokal & Paket Wisata**
4. Pemesanan Tiket Wisata & Event (E-Ticket)

Platform ini menghubungkan wisatawan dengan **Penyedia Jasa Lokal (Agensi)** di setiap daerah, selain menyediakan hotel dan tiket masuk.
Fokus: **Stay, Explore, & Experience with Locals**.

Website harus terlihat premium, trustworthy, visual-heavy, dan clean.

====================================================

🎨 DESIGN REQUIREMENT

Style:
- Modern & Immersive
- Clean Layout
- Visual-heavy (Banyak penggunaan gambar berkualitas tinggi)
- Glassmorphism accent
- Rounded corner
- Smooth transition

Primary Color:
#059669 (Emerald Green - Nuansa Alam)
Secondary: #0284C7 (Sky Blue - Nuansa Profesional/Trust untuk Hotel & Agensi)
Accent: #D97706 (Amber - Nuansa Senja/Budaya)

Font:
Plus Jakarta Sans / Inter

UI Principles:
- Mobile first
- Responsive
- Search Bar yang prominent (Destinasi/Hotel/Paket Tour)
- Booking flow yang mudah dan aman

====================================================

🚀 FITUR UTAMA PLATFORM

====================================
1️⃣ EKSPLORASI DESTINASI (WISATA)
====================================

Fitur:
- Search destinasi
- Filter (Kategori: Pantai, Gunung, Sejarah, Kuliner)
- Filter Lokasi
- Card destinasi immersive
- Detail Destinasi (Galeri, Peta, Harga Tiket, Fasilitas)

Halaman:
- /wisata
- /wisata/:slug

Komponen:
- FilterWisata
- CardDestinasi
- DetailDestinasi

====================================
2️⃣ HOTEL & AKOMODASI
====================================

Fitur:
- Search Hotel (Lokasi, Tanggal Check-in/out)
- Filter (Bintang, Harga, Fasilitas)
- Card Hotel Modern
- Detail Hotel (Kamar, Review)

Halaman:
- /hotel
- /hotel/:slug

Komponen:
- SearchHotelWidget
- CardHotel
- DetailHotel

====================================
3️⃣ AGENSI TRAVEL & PAKET WISATA
====================================

Fitur:
- **Direktori Agensi per Lokasi** (Misal: Agensi di Jogja, Agensi di Bali)
- Profil Agensi (Rating, Review, Lisensi, Daftar Paket)
- **Listing Paket Wisata** (Open Trip / Private Trip)
- Filter Paket (Durasi: 3D2N, Harga, Tipe)
- Detail Paket (Itinerary Harian, Termasuk/Tidak Termasuk, Meeting Point)

Halaman:
- /agensi (List semua agensi / paket)
- /agensi/:id (Profil Agensi)
- /paket/:slug (Detail Paket Wisata)

Komponen:
- CardAgensi
- CardPaketWisata
- FilterPaket
- ItineraryList

====================================
4️⃣ EVENT & BUDAYA
====================================

Fitur:
- Kalender Event
- Daftar Festival / Pentas Seni
- Detail Event

Halaman:
- /acara
- /acara/:slug

====================================
5️⃣ BOOKING SYSTEM (ALL-IN-ONE)
====================================

Fitur:
- Cart / Checkout universal
- Ringkasan Pesanan (Hotel/Tiket/Paket Wisata)
- Form Data Tamu
- Simulasi Pembayaran
- E-Voucher

Halaman:
- /booking/checkout
- /booking/sukses

====================================
6️⃣ DASHBOARD WISATAWAN (USER)
====================================

Fitur:
- Riwayat Pemesanan
- Voucher Saya
- Wishlist

Halaman:
- /user/dashboard

====================================================

📁 PROJECT STRUCTURE WAJIB MENGIKUTI INI

(Lihat file hirarki.md untuk detail struktur folder)

====================================================

📦 DATA STRUCTURE (CONCEPT)

User:
- id, name, email, phone, avatar

Destination:
- id, slug, name, description, location, category, rating, price, images[], facilities[]

Hotel:
- id, slug, name, type, stars, location, priceStart, rating, rooms[]

Agency (Agentur):
- id, slug, name, location (Base City), logo, description, rating, verified (bool), contactInfo

TourPackage:
- id, slug, agencyId, title, type (OpenTrip/Private), duration (e.g., "3D2N"), price, location, itinerary[], facilities[], images[]

Booking:
- id, userId, type (HOTEL/TICKET/TOUR), itemId, date, quantity, totalPrice, status

====================================================

📊 BERANDA HARUS MENAMPILKAN

- Hero Section Immersive dengan Tab Pencarian (Wisata / Hotel / Paket Tour)
- Promo Eksklusif
- Destinasi Trending
- **Rekomendasi Paket Wisata (Best Tours)**
- **Agensi Lokal Terpopuler**
- Rekomendasi Hotel Pilihan
- Testimoni

====================================================

🎯 OUTPUT YANG DIHARAPKAN

AI harus menghasilkan:

1. Struktur folder lengkap sesuai hirarki.md
2. Komponen React TypeScript
3. Tailwind styling modern
4. Dummy data untuk:
   - 4 Destinasi
   - 3 Hotel
   - **3 Agensi Travel & 4 Paket Wisata (Jogja/Bali)**
5. Routing menggunakan React Router
6. State management untuk Booking flow

====================================================

GOAL AKHIR:

Website menjadi ekosistem pariwisata lengkap.
User bisa pesan hotel sendiri, ATAU pesan paket tour dari agensi lokal jika tidak mau ribet.
Profesional, clean, scalable.

END OF PROMPT