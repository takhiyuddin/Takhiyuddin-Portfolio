# ./Takhiyuddin.com - Professional Portfolio

Repositori ini berisi kode sumber statis untuk halaman portofolio profesional **Takhiyuddin.com**. Portofolio ini menampilkan rekam jejak pengembangan perangkat lunak (khususnya ekosistem Apple/iOS dan web) dengan fokus utama pada sektor **Pertambangan serta Minyak & Gas (Mining, Oil & Gas)** dan **Pelayanan Publik**.

Halaman web ini dibangun menggunakan desain *timeline* vertikal yang responsif, bersih, dan dilengkapi dengan animasi interaktif.

## 🛠️ Teknologi Pembuatan Web
Portofolio ini dibangun murni menggunakan pendekatan *front-end* statis yang ringan dan cepat:
- **HTML5 & CSS3** (Custom Timeline UI)
- **Bootstrap 5.3.0** (Grid system, Accordion, dan Typography)
- **Bootstrap Icons** (Ikonografi UI)
- **AOS (Animate On Scroll)** (Animasi transisi elemen)

---

## 🚀 Etalase Proyek (Project Showcase)

### 🏗️ Sektor Pertambangan serta Minyak & Gas

#### 1. TataBumi - Mining Operations ERP (v5.0)
Aplikasi *Enterprise Resource Planning* (ERP) komprehensif untuk memonitor produksi dari pit ke pelabuhan (*Pit to Port*) dan manajemen aset alat berat.
- **Teknologi:** SwiftUI, Combine (MVVM), Swift Charts, MapKit.
- **Sorotan Utama:**
  - Arsitektur *Router-based View* untuk skalabilitas modul (Produksi, IoT, Logistik, HR).
  - Implementasi IoT & Geotagging menggunakan *Custom* `MKMapView` dan WebSocket real-time.
  - Optimasi *memory leak* pada MapKit dengan *clustering* untuk 1000+ anotasi aset.

#### 2. Nirwana - Environmental Management & ESG Analytics (v4.0)
Portal *Dual-Role* untuk pelaporan manifest limbah, audit emisi karbon, dan reklamasi lahan.
- **Teknologi:** SwiftUI, Charts Data-Viz, CoreLocation.
- **Sorotan Utama:**
  - Desain *High-Visibility UI* untuk kondisi lapangan (sinar matahari terik).
  - Reaktivitas peringatan bahaya (*Hazard Alert*) dari input sampel air (pH & TSS) otomatis.
  - Kompresi *payload* API dan perbaikan akurasi `CoreLocation` untuk data manifest.

#### 3. KendaliBBM - Enterprise Fuel Monitoring System (v3.0)
Sistem pengawasan distribusi pasokan solar dari truk tangki ke armada alat berat untuk mencegah kecurangan dan kebocoran.
- **Teknologi:** SwiftUI, Combine, Rule-Engine.
- **Sorotan Utama:**
  - Modul *Security Audit* berdasarkan analisis *Burn Rate* mesin.
  - Pembuatan *Circular Capacity Gauge* dinamis menggunakan `Path` dan `AnimatableData`.
  - Refaktor alur *Publisher* Combine untuk efisiensi pemanggilan API jaringan.

#### 4. SentriSpace - Confined Space Entry Monitor (v2.0)
Platform pemantauan Keselamatan dan Kesehatan Kerja (K3) bagi pengawas *Hole Watcher* di ruang terbatas.
- **Teknologi:** SwiftUI, Live Timers, Safety-First UI.
- **Sorotan Utama:**
  - *Live Timers* presisi yang berjalan di *background state* tanpa membebani *Main Thread*.
  - Sistem Pemicu Alarm Evakuasi otomatis terintegrasi dengan *Haptic Feedback* (`UIImpactFeedbackGenerator`).
  - Validasi lokal pendeteksi batas gas (LEL, H2S, O2).

#### 5. Estafet - Digital Shift Handover System (v1.0)
Aplikasi peralihan operasional (*handover*) antar-shift untuk menghapus ketergantungan pada pencatatan kertas fisik.
- **Teknologi:** SwiftUI, State Management.
- **Sorotan Utama:**
  - *Acknowledgment Workflow* yang mengamankan serah terima dengan tanda tangan digital & PIN.
  - Pemodelan *State* menggunakan Enum Tersandi (`Normal`, `Warning`, `Breakdown`).
  - Optimasi sinkronisasi *NavigationStack* saat konfirmasi *multi-user* bersamaan.

---

### 🏛️ Sektor Pelayanan Publik

#### 1. BAZNAS Jateng - ZIS Management Portal (v2.0)
Platform pelayanan publik terpadu untuk pengumpulan dan pendistribusian Zakat, Infak, dan Sedekah (ZIS) di Provinsi Jawa Tengah.
- **Teknologi:** Bootstrap 5, Laravel (MVC), MySQL, Payment Gateway.
- **Sorotan Utama:**
  - Arsitektur basis data terpusat antar BAZNAS Kabupaten/Kota.
  - UI/UX *Accessibility-friendly* dengan navigasi *Floating Dock* dan *Multi-channel Payment Gateway*.
  - Penanganan performa (*Load Balancing*) untuk lonjakan *traffic* donatur di bulan Ramadhan dan implementasi kompresi WebP.

---

## 💻 Cara Menjalankan (Local Development)

Karena web ini menggunakan file HTML statis dengan CDN, Anda tidak memerlukan proses *build* atau instalasi *package*. 
1. *Clone* repositori ini.
2. Pastikan Anda memiliki folder `assets/` di *root directory* yang berisi gambar-gambar proyek (`TataBumi.png`, `Nirwana.png`, `KendaliBBM.png`, `SentriSpace.png`, `Estafet.png`, dan `Baznas Jateng.png`).
3. Buka file `index.html` langsung di *browser* pilihan Anda (Chrome, Safari, Firefox).
