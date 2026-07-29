# ./Takhiyuddin.com - Developer Portfolio

Selamat datang di repositori portofolio **Takhiyuddin.com**. Dokumen ini merangkum berbagai proyek pengembangan perangkat lunak yang telah dibangun, mencakup aplikasi *mobile* dan *web* di berbagai sektor industri mulai dari Pertambangan & Migas, Pelayanan Publik, hingga E-Commerce.

---

## 🏭 Mining and Oil & Gas

### TataBumi - Mining Operations ERP (v5.4.2)
*   **Periode:** 2024 - 2026
*   **Teknologi:** SwiftUI, Combine (MVVM), Swift Charts, MapKit
*   **Deskripsi:** Aplikasi *Enterprise Resource Planning* (ERP) komprehensif untuk sektor pertambangan dengan arsitektur *Router-based View* yang modular.
*   **Fitur Utama:** Monitoring produksi *Pit to Port* *real-time*, manajemen aset alat berat, manajemen multi-user (RBAC), dan integrasi *geotagging* MapKit untuk melacak pergerakan aset.
*   **Pencapaian Teknis:** Menerapkan MVVM murni, menyelesaikan *memory leak* pada MapKit saat memuat 1000+ anotasi, dan mengoptimalkan *rendering* Swift Charts dari O(n²) ke O(n).

### Nirwana - Environmental Management & ESG Analytics (v4.0)
*   **Rilis:** Oktober 2025
*   **Teknologi:** SwiftUI, Charts Data-Viz, CoreLocation
*   **Deskripsi:** Portal *Dual-Role* untuk memfasilitasi akses lapangan dan *Dashboard Executive* terkait pengelolaan lingkungan dan audit ESG.
*   **Fitur Utama:** Audit lingkungan otomatis (emisi karbon, limbah B3, reklamasi), pelaporan insiden instan, dan pemicu *Hazard Alert* otomatis untuk sampel air di luar ambang batas.
*   **Pencapaian Teknis:** Mengurangi ukuran *payload* API sebesar 40% dengan kompresi JSON sisi klien dan mendesain UI dinamis yang adaptif di bawah sinar matahari lapangan.

### KendaliBBM - Enterprise Fuel Monitoring System (v3.0)
*   **Rilis:** Mei 2025
*   **Teknologi:** SwiftUI, Combine, Rule-Engine
*   **Deskripsi:** Sistem pengontrol distribusi pasokan solar dari Truk Tangki ke armada alat berat di area tambang.
*   **Fitur Utama:** Pencatatan meteran digital via QR/Barcode, deteksi anomali konsumsi (*Burn Rate*), dan modul *Security Audit* finansial.
*   **Pencapaian Teknis:** Membangun *Circular Capacity Gauge* reaktif dan menerapkan *Rule-Engine* sisi klien untuk mencegah *over-capacity input* secara instan.

### SentriSpace - Confined Space Entry Monitor (v2.0)
*   **Rilis:** Januari 2025
*   **Teknologi:** SwiftUI, Live Timers, Safety-First UI
*   **Deskripsi:** Platform monitoring *Health & Safety* (HSE) khusus pengawas keselamatan ruang terbatas (*Hole Watcher*).
*   **Fitur Utama:** Manajemen izin kerja (*Permit to Work*), pencatatan durasi *shift* presisi, dan pemicu alarm evakuasi otomatis.
*   **Pencapaian Teknis:** Memanfaatkan *Native Timer* SwiftUI agar berjalan persisten di *background* tanpa membebani *Main Thread*, serta integrasi *Haptic Feedback* untuk peringatan darurat.

### Estafet - Digital Shift Handover System (v1.0)
*   **Rilis:** Agustus 2024
*   **Teknologi:** SwiftUI, State Management
*   **Deskripsi:** Aplikasi peralihan operasional (*handover*) antar-shift untuk meminimalkan risiko kehilangan data serah terima alat.
*   **Fitur Utama:** *Acknowledgment Workflow* ketat, validasi tanda tangan digital via PIN, dan *dashboard* mandor terpusat.
*   **Pencapaian Teknis:** Memodelkan status operasional dengan Swift Enum tersandi dan migrasi ke `@StateObject` untuk mengatasi masalah UI yang tidak melakukan *re-render*.

---

## 🏛️ Public Services

### BAZNAS Jateng - ZIS Management Portal (v2.0)
*   **Rilis:** Maret 2024
*   **Teknologi:** Bootstrap 5, Laravel (MVC), MySQL, Payment Gateway
*   **Deskripsi:** Platform pelayanan publik terpadu untuk optimalisasi pengumpulan dan pendistribusian Zakat, Infak, dan Sedekah (ZIS) di Jawa Tengah.
*   **Fitur Utama:** Sistem manajemen keuangan transparan, pendataan mustahik berbasis wilayah, integrasi *Multi-channel Payment Gateway*, dan layanan CS responsif.
*   **Pencapaian Teknis:** Optimasi *Load Balancing* server untuk lonjakan *traffic* Ramadhan dan penerapan *lazy loading* / WebP untuk performa halaman.

### Jemputin - Circular Economy & Waste Management (v1.0)
*   **Rilis:** November 2023
*   **Teknologi:** HTML/CSS/JS, Bootstrap 5, Chart.js, Leaflet.js
*   **Deskripsi:** Platform sirkular ekonomi untuk daur ulang sampah dengan layanan penjemputan dari rumah.
*   **Fitur Utama:** Kalkulator Emisi CO2, konversi poin *reward* (*QRIS/E-Wallet*), direktori Bank Sampah berbasis peta interaktif, dan modul edukasi.
*   **Pencapaian Teknis:** Integrasi Leaflet.js untuk pemetaan presisi dan manajemen *state* serta autentikasi lokal berbasis JSON di `LocalStorage`.

---

## 🛍️ E-Commerce

### AppleNation - Premium Apple Store App (v1.0)
*   **Rilis:** April 2026
*   **Teknologi:** SwiftUI, Combine, State Management, JSON Encoding
*   **Deskripsi:** Aplikasi *e-commerce* eksklusif ekosistem Apple dengan antarmuka bertema *Glassmorphism*.
*   **Fitur Utama:** Katalog interaktif dengan filter dinamis, animasi harga *real-time* berbasis varian, dan sistem *checkout* terintegrasi.
*   **Pencapaian Teknis:** Penggunaan `EnvironmentObject` global untuk sinkronisasi state keranjang/pesanan dan penerapan persistensi data lokal otomatis via `UserDefaults`.

---

## 🛠️ Ringkasan Teknologi

| Kategori | Teknologi Utama |
| :--- | :--- |
| **iOS / Apple Platforms** | SwiftUI, Combine, Swift Charts, MapKit, CoreLocation |
| **Arsitektur Mobile** | MVVM, Router-based View, State Management, Rule-Engine |
| **Web Frontend** | HTML/CSS/JS, Bootstrap 5, Chart.js, Leaflet.js |
| **Backend & Database** | Laravel (MVC), MySQL, REST API Integration |
| **Integrasi Eksternal** | Payment Gateway, IoT WebSocket, Geotagging |

<br>

*Dokumen ini dihasilkan berdasarkan portofolio interaktif pada ./Takhiyuddin.com.*
