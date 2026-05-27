# 🏥 Sistem Pendaftaran Online
Aplikasi berbasis web (Client-Side) yang dirancang untuk mempermudah proses pendaftaran pasien secara mandiri di Klinik. Project ini dibuat menggunakan HTML5, CSS3 (Tailwind-inspired styling), dan JavaScript.

## 🚀 Live Demo
🔗 [Lihat Web Pendaftaran Di Sini](https://nabilsyah57.github.io/clinic-online-registration-system) 

## ✨ Fitur Utama
- **Sistem Alur 5 Langkah (Step-by-Step):** Memandu pasien dari memilih tipe identitas hingga mendapatkan nomor antrian.
- **Formulir Dinamis:** Form otomatis berubah berdasarkan kategori pasien (Dewasa/Anak).
- **Manajemen Slot Kuota:** Pencegahan *double-booking* menggunakan slot waktu terintegrasi dengan `localStorage`.
- **Konfirmasi WhatsApp:** Menghasilkan teks otomatis terformat tebal/miring untuk dikirim langsung ke WhatsApp admin klinik.
- **Fitur Cetak Mandiri:** Layout otomatis menyesuaikan (*print-optimized*) saat pasien ingin mencetak bukti antrian.

## ⚙️ Cara Konfigurasi (Untuk Pengelola Klinik)
Buka file `index.html` dan sesuaikan objek `KLINIK` pada baris awal tag `<script>` dengan data klinik Anda:

```javascript
const KLINIK = {
  nama: 'NAMA KLINIK ANDA',
  alamat: 'ALAMAT LENGKAP KLINIK',
  telepon: 'NOMOR TELEPON',
  whatsapp: '628xxxxxxxxxx', // Format kode negara tanpa '+'
  maps_url: 'LINK GOOGLE MAPS KLINIK',
  daftar_url: 'URL WEBSITE INI',
  kuota_per_slot: 3, // Batas pasien per jam
  dokter: 'Nama Dokter yang Bertugas',
};
