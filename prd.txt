Tentu, ini adalah **Product Requirements Document (PRD)** yang detail untuk proyek *mid-term* kamu. Konsep yang dipilih adalah **Medis**, dengan fokus pada kemudahan navigasi dan visual yang bersih agar nyaman di mata (user-friendly).

---

# PRD: MediHub – Modern Medical Dashboard

**MediHub** adalah platform manajemen layanan kesehatan sederhana yang dirancang untuk mempermudah pasien dalam melihat riwayat medis dan melakukan janji temu dengan dokter secara efisien.
    
---

## 1. Informasi Proyek
* **Target Platform:** Web (Hosting di GitHub Pages).
* **Jumlah Halaman:** 3 Halaman Utama.
* **Teknologi:** HTML5, CSS3 (Tailwind CSS), dan JavaScript.
* **Tim:** Minimal 4 Orang (Project Manager, UI/UX Designer, Frontend Dev 1, Frontend Dev 2).

---

## 2. Struktur Halaman (Sitemap)

| Halaman | Komponen Wajib | Deskripsi |
| :--- | :--- | :--- |
| **1. Beranda (Dashboard)** | Ringkasan Layanan | Visualisasi informasi umum, statistik kesehatan singkat, dan navigasi utama. |
| **2. Riwayat Medis (Records)** | **Tabel (Table)** | Menampilkan data pasien, jadwal kontrol, atau riwayat diagnosa dalam format tabel yang rapi. |
| **3. Janji Temu (Booking)** | **Formulir (Form)** | Formulir pendaftaran janji temu dokter (Input nama, poli, tanggal, dan keluhan). |

---

## 3. Spesifikasi Fitur & Fungsionalitas

### A. Halaman Beranda (Home)
* **Navigation Bar:** Menggunakan desain *floating capsule* yang minimalis untuk berpindah antar halaman.
* **Hero Section:** Pesan selamat datang dan ringkasan status rumah sakit/klinik.
* **Fitur Pendukung:** Kartu informasi (Bento Grid style) yang menampilkan jam operasional dan dokter yang sedang bertugas.

### B. Halaman Riwayat Medis (Table Page)
* **Data Table:** Menampilkan daftar riwayat pemeriksaan.
* **Kolom Tabel:** No, Tanggal, Nama Dokter, Spesialisasi, dan Status (Selesai/Pending).
* **Styling:** Tabel menggunakan *zebra-striping* lembut untuk kenyamanan membaca.

### C. Halaman Janji Temu (Form Page)
* **Input Fields:**
    * Nama Lengkap (Text)
    * Nomor Rekam Medis (Number)
    * Pilih Spesialis (Dropdown/Select)
    * Tanggal Perjanjian (Date Picker)
    * Keluhan Singkat (Textarea)
* **Validation:** Pesan sukses muncul menggunakan JavaScript setelah form dikirim (*submitted*).

---

## 4. Panduan Desain (Visual Style)

Untuk mencapai desain yang "nyaman di mata" dan profesional, berikut adalah panduan estetikanya:

* **Tema Warna:** Dominasi **Putih dan Abu-abu sangat muda** (Off-white) untuk latar belakang, dengan **Aksen Hitam atau Biru Gelap** untuk teks dan elemen penting.
* **Tipografi:** Gunakan font Sans-serif yang bersih (seperti Inter atau Geist) agar teks medis mudah dibaca.
* **Layout:** Menggunakan **Bento Grid** untuk menyusun informasi agar terlihat modern dan tidak menumpuk.
* **Animasi:** Transisi halus saat perpindahan halaman atau hover pada tombol untuk memberikan kesan interaktif yang elegan.

---

## 5. Implementasi Teknis (Stack)

* **Framework CSS:** Menggunakan **Tailwind CSS** (melalui CDN agar kompatibel langsung dengan GitHub Pages). Tailwind memudahkan pengaturan *spacing* dan *responsiveness*.
* **Icons:** Lucide Icons atau Phosphor Icons untuk memperkuat visual medis.
* **Deployment:** Repository akan dihosting di `username.github.io/nama-proyek`.

---

## 6. Pembagian Tugas (Saran)

1.  **Anggota 1 (Lead & UI):** Menyusun struktur HTML dasar dan menentukan sistem warna/layout.
2.  **Anggota 2 (Frontend - Halaman Tabel):** Fokus pada pembuatan tabel data dan memastikan responsivitas di perangkat mobile.
3.  **Anggota 3 (Frontend - Halaman Form):** Fokus pada fungsionalitas formulir dan validasi input.
4.  **Anggota 4 (JS & Integration):** Menangani logika navigasi (SPA sederhana), interaksi klik, dan deployment ke GitHub Pages.

---

### Tips Pengembangan
Untuk GitHub Pages, pastikan semua file gambar berada dalam folder `assets` dan gunakan *relative path* (seperti `./css/style.css`) agar file terbaca dengan benar saat diunggah. 

Apakah kamu ingin dibuatkan *boilerplate* kode HTML dasar untuk struktur 3 halaman ini?