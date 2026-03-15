

🏆 Student Achievement Dashboard (v1.0)
Dashboard interaktif untuk memonitoring dan mengelola data prestasi siswa secara real-time. Proyek ini menggunakan Google Sheets sebagai Database dan Google Apps Script sebagai API, memberikan solusi serverless yang ringan namun bertenaga.

🚀 Fitur Utama
Real-time Data Sync: Terhubung langsung dengan Google Sheets via Apps Script API.

Dynamic Analytics: Kurva tren juara tahunan otomatis menggunakan Chart.js.

Modern UI/UX: Dibangun dengan Tailwind CSS dengan mode gelap (dark mode) yang elegan.

Responsive Design: Tampilan optimal di perangkat mobile, tablet, maupun PC.

Interactive Modal: Klik pada nama siswa untuk melihat detail lengkap prestasi secara akurat.

Quick Search & Filter: Memudahkan pencarian data berdasarkan nama, NISN, atau bidang lomba.

🛠️ Tech Stack
Frontend: HTML5, Tailwind CSS, JavaScript (ES6+).

Charts: Chart.js.

Backend/API: Google Apps Script (GAS).

Database: Google Sheets.

Hosting: Vercel / GitHub Pages.

📖 Cara Penggunaan
1. Persiapan Google Sheets
Buat Google Sheets baru dengan nama sheet Form_Responses.

Pastikan header kolom di baris pertama adalah: Timestamp, Nama Siswa, Nisn, Cabang Lomba, BIDANG LOMBA, JUARA LOMBA, TAHUN.

2. Deploy API (Google Apps Script)
Buka Extensions > Apps Script.

Copy-paste kode dari kode.gs ke editor.

Klik Deploy > New Deployment.

Pilih jenis Web App, set Execute as ke Me, dan Who has access ke Anyone.

Copy Web App URL yang dihasilkan.

3. Konfigurasi Frontend
Buka file index.html.

Cari variabel const API_URL dan ganti dengan URL yang Anda copy tadi.

JavaScript
const API_URL = "URL_APPS_SCRIPT_ANDA_DISINI";
4. Hosting ke Vercel/GitHub Pages
Push folder proyek ini ke repository GitHub Anda.

Hubungkan repository tersebut ke Vercel.

Vercel akan secara otomatis mendeteksi file index.html dan melakukan deployment.

📂 Struktur File
Bash
.
├── index.html    # Tampilan utama & Logika Frontend
├── kode.gs       # Logic API untuk Google Apps Script
└── README.md     # Dokumentasi proyek
📝 Catatan Engineer
Pastikan setiap kali Anda melakukan perubahan pada kode.gs, Anda melakukan New Deployment atau melakukan Manage Deployment ke versi terbaru agar perubahan API tersinkronisasi dengan Frontend.

input data : https://forms.gle/KpsB6MngNDTsXANG6

Developed with ❤️ for Education Management.
