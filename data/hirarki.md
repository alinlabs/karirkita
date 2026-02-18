PROJECT STRUCTURE
├── App.tsx
├── constants.ts              # Data dummy (Destinasi, Hotel, Agensi, Paket, User)
├── index.css
├── index.html
├── index.tsx
├── package.json
├── postcss.config.js
├── README.md
├── tailwind.config.js
├── tsconfig.json
├── types.ts                  # Interface TS (Destination, Hotel, Agency, Package, Booking)
├── vite-env.d.ts
├── vite.config.ts
├── config/
│   ├── menu.ts               # Konfigurasi Menu Navigasi
│   └── site.ts               # Metadata Website
├── halaman/
│   ├── beranda/              # Halaman Depan
│   │   ├── Hero.tsx          # With Tabs (Wisata/Hotel/Tour)
│   │   ├── SearchWidget.tsx  # Komponen Tab Pencarian
│   │   ├── SectionHotel.tsx
│   │   ├── SectionPaket.tsx  # Rekomendasi Paket Wisata
│   │   ├── SectionAgensi.tsx # Rekomendasi Agensi
│   │   └── Container.tsx
│   ├── wisata/               # Halaman Eksplorasi Destinasi
│   │   ├── CardDestinasi.tsx
│   │   ├── FilterWisata.tsx
│   │   ├── DetailDestinasi.tsx
│   │   └── Container.tsx
│   ├── hotel/                # Halaman Hotel & Akomodasi
│   │   ├── CardHotel.tsx
│   │   ├── FilterHotel.tsx
│   │   ├── DetailHotel.tsx
│   │   ├── RoomList.tsx
│   │   └── Container.tsx
│   ├── agensi/               # Halaman Agensi & Paket Wisata
│   │   ├── CardAgensi.tsx    # Kartu Profil Agensi
│   │   ├── CardPaket.tsx     # Kartu Paket Wisata
│   │   ├── FilterAgensi.tsx  # Filter Paket/Agensi
│   │   ├── DetailAgensi.tsx  # Halaman Profil Agensi
│   │   ├── DetailPaket.tsx   # Halaman Detail Paket Tour
│   │   └── Container.tsx     # List Agensi/Paket
│   ├── acara/                # Halaman Event/Budaya
│   │   ├── CardEvent.tsx
│   │   ├── DetailEvent.tsx
│   │   └── Container.tsx
│   ├── pemesanan/            # Flow Booking Universal
│   │   ├── Checkout.tsx
│   │   ├── PaymentSim.tsx
│   │   └── Sukses.tsx
│   ├── user/                 # Dashboard Wisatawan
│   │   ├── UserLayout.tsx
│   │   ├── Dashboard.tsx
│   │   ├── PesananSaya.tsx
│   │   └── Wishlist.tsx
│   ├── auth/
│   │   ├── Login.tsx
│   │   └── Register.tsx
│   ├── legal/
│   │   └── PrivacyPolicy.tsx
│   └── error/
│       └── NotFound.tsx
├── hooks/
│   ├── useAuth.ts
│   ├── useBooking.ts
│   ├── useSearch.ts
│   └── useScrollTop.ts
├── komponen/
│   ├── ui/                   # Atomic Components
│   │   ├── Button.tsx
│   │   ├── Card.tsx
│   │   ├── Badge.tsx
│   │   ├── Input.tsx
│   │   ├── Rating.tsx
│   │   └── Modal.tsx
│   └── umum/                 # Global Components
│       ├── Layout.tsx
│       ├── Navbar.tsx
│       ├── Footer.tsx
│       └── DatePicker.tsx
├── public/
│   ├── data/                 # JSON / MD Files
│   └── images/               # Assets
├── services/                 # Mock API Services
│   ├── wisataService.ts
│   ├── hotelService.ts
│   ├── agensiService.ts      # Service Agensi & Paket
│   └── bookingService.ts
└── utils/
    ├── cn.ts
    ├── formatRupiah.ts
    └── formatDate.ts