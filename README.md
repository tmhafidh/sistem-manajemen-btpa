#Monitor BTPA (Dokumentasi Proyek)
Monitor BTPA adalah aplikasi dashboard manajemen operasional yang dirancang khusus untuk memantau siklus hidup dokumen BTPA (Bukti Terima Penimbangan Ayam) di lingkungan operasional lapangan. Aplikasi ini membantu tim admin dan pengawas kandang dalam melacak dokumen dari tahap distribusi ke tim lapangan hingga proses panen selesai.

🚀 Fitur Utama
Analitik Dasbor Real-time: Visualisasi distribusi status dokumen (Laci Admin, Di Lapangan, Di Penimbang, Terpakai).

Manajemen Siklus Kandang (Chick-in): Sistem alokasi otomatis dokumen ke kandang dengan validasi real-time.

Manajemen Inventaris: Pengelolaan stok dokumen di laci admin dan pelacakan dokumen yang sedang dipegang oleh petugas penimbang.

Scan Massal (Global): Validasi dua tahap untuk memproses penyelesaian status dokumen secara massal dengan laporan akurat.

Navigasi Cerdas: Pencarian global yang memungkinkan navigasi instan ke lokasi spesifik dokumen (kandang, laci, atau penimbang).

Keamanan Data: Sistem Backup dan Restore berbasis file JSON untuk menjaga integritas data Anda.

🛠️ Teknologi yang Digunakan
Proyek ini dibangun dengan pendekatan single-file application untuk portabilitas maksimal tanpa memerlukan build step yang kompleks:

React 18: Core framework untuk komponen UI yang reaktif.

Tailwind CSS: Utility-first CSS framework untuk desain antarmuka yang modern dan responsif.

Lucide React: Pustaka ikon yang bersih dan ringan.

Babel Standalone: Memungkinkan penulisan sintaks JSX langsung di dalam peramban (browser).

LocalStorage API: Penyimpanan data lokal yang cepat dan persistent di sisi klien.

📂 Struktur Data
Data aplikasi dikelola dalam format JSON dengan entitas utama:

Teams: Master data tim (PPL & Penimbang).

Batches: Data kandang dan riwayat siklus panen.

Documents: Log individu untuk setiap nomor BTPA beserta status posisinya.

💡 Panduan Penggunaan
1. Inisialisasi
Aplikasi dapat langsung dijalankan hanya dengan membuka file index.html di peramban modern (Chrome/Edge/Firefox).

Pastikan koneksi internet tersedia untuk memuat dependensi dari CDN (React, Tailwind, Lucide).

2. Alur Kerja Utama
Input Data Tim: Pastikan data tim sudah terinput di menu Master Data Tim.

Input Stok: Masukkan rentang nomor BTPA ke Gudang (Stok Internal) untuk mengaktifkan dokumen tersebut di sistem.

Chick-in: Saat panen dimulai, gunakan menu Buka Kandang untuk mengalokasikan stok dari laci ke kandang spesifik.

Monitoring: Gunakan fitur Search untuk mencari posisi dokumen secara cepat.

Scan Selesai: Saat panen, gunakan Scan Massal untuk mengubah status dokumen menjadi "Terpakai" secara otomatis.

📦 Backup & Pemulihan
Disarankan untuk melakukan Backup secara berkala melalui menu Database. Anda cukup menekan tombol "Ekspor Data JSON" dan simpan file tersebut sebagai cadangan.

Proyek ini dikembangkan sebagai solusi optimasi administrasi operasional. Untuk pengembangan lebih lanjut atau pertanyaan teknis, silakan merujuk pada dokumentasi kode di dalam index.html.
