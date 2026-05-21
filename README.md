📊 Monitor BTPA

Sistem Digital Manajemen Dokumen Bukti Terima Penimbangan Ayam (BTPA)

Monitor BTPA adalah aplikasi antarmuka dasbor operasional (operational dashboard) berbasis web yang dirancang khusus untuk memantau, melacak, dan mengelola siklus hidup dokumen BTPA. Aplikasi ini membantu tim admin dan pengawas kandang melacak perpindahan dokumen—mulai dari gudang pusat (Laci Admin), diserahkan ke Penimbang, dialokasikan ke Kandang (Chick-in), hingga akhirnya berstatus Sah (Selesai Terpakai).

✨ Fitur Utama

Aplikasi ini dilengkapi dengan berbagai fitur cerdas untuk mempercepat proses entri data dan meminimalisir human error:

📈 Dasbor Analitik Global & Per-Tim: Visualisasi data real-time menggunakan persentase distribusi dan statistik dokumen (Selesai, Di Laci, Di Penimbang, Menggantung di Lapangan).

👥 Master Data Tim: Pengelolaan kombinasi staf lapangan (Petugas Penyuluh Lapangan / PPL & Penimbang) secara dinamis.

📦 Manajemen Gudang (Laci Admin): Sistem inventaris cerdas yang melacak sisa ketersediaan dokumen dan fitur handover (serah terima) dokumen resmi ke Penimbang.

🐣 Buka Kandang (Chick-in) dengan Smart Click-to-Fill: Sistem alokasi rentang dokumen super cepat. Pengguna cukup mengklik ketersediaan grup nomor BTPA di Laci, dan kolom rentang otomatis terisi tanpa harus mengetik manual.

🚜 Proses Panen (Kandang Aktif): Manajemen siklus panen. Menampilkan dokumen mana yang belum dikembalikan (Menggantung) beserta eksekusi status massal.

📠 Scan Massal (Global) Validasi 2 Tahap: Mendukung copy-paste ratusan nomor sekaligus dari Excel/WhatsApp. Memiliki sistem preview untuk memisahkan dokumen yang valid, ilegal (tidak ditemukan), dan yang sudah diproses sebelum melakukan eksekusi final.

🔍 Pencarian Cerdas (Smart Global Search): Cari nomor BTPA, dan sistem akan langsung mengarahkan pengguna ke halaman spesifik (Kandang/Laci) di mana dokumen tersebut berada.

💾 Database Management: Menggunakan mesin useSyncStorage yang menyimpan data instan tanpa lag ke LocalStorage browser. Dilengkapi fitur Backup (Ekspor ke JSON) dan Restore (Impor dari JSON).

🛠️ Teknologi yang Digunakan

Proyek ini dibangun menggunakan arsitektur Single-File Web Application. Sangat portabel, tidak memerlukan instalasi server atau npm, dan bisa langsung dijalankan di semua browser modern.

React 18 (melalui Babel Standalone)

Tailwind CSS (via CDN untuk desain antarmuka modern & responsif)

Lucide React (Pustaka ikon antarmuka yang tajam dan konsisten)

HTML5 & LocalStorage API (Manajemen state persisten)

🚀 Cara Penggunaan (Zero Setup)

Aplikasi ini dirancang plug-and-play. Tidak ada prasyarat instalasi perangkat lunak tambahan.

Unduh atau simpan file index.html.

Klik ganda pada file index.html untuk membukanya melalui peramban (Rekomendasi: Google Chrome, Microsoft Edge, atau Mozilla Firefox).

Pastikan perangkat Anda terhubung ke internet untuk pertama kali dibuka, agar pustaka React dan Tailwind dapat dimuat dari CDN.

Data Anda akan tersimpan secara otomatis dan aman di dalam peramban (LocalStorage).

📂 Alur Kerja Disarankan (Workflow)

Daftarkan Tim: Masuk ke menu Master Data Tim dan buat minimal satu tim kombinasi PPL dan Penimbang.

Tambah Stok: Masuk ke menu Tambah Stok Laci, ketik rentang dokumen kosong yang baru saja dicetak/diterima dari pusat untuk dialokasikan ke tim.

Buka Kandang: Masuk ke menu 1. Buka Kandang (Input), masukkan data populasi ayam, dan alokasikan dokumen dari Laci ke kandang tersebut.

Tutup Siklus / Scan: Saat panen berlangsung, gunakan menu Scan Massal atau 2. Proses Panen Aktif untuk menyahkan dokumen yang telah dipakai.

⚠️ Peringatan Keamanan Data

Karena aplikasi ini berjalan sepenuhnya di sisi klien (Client-side):

JANGAN menghapus riwayat peramban (Clear Browsing Data / Cache & Cookies) Anda secara sembarangan, karena akan menghapus data operasional BTPA Anda.

LAKUKAN BACKUP RUTIN: Masuk ke menu Backup & Restore dan klik Unduh Backup setiap kali Anda selesai melakukan banyak perubahan data. Simpan file .json tersebut di tempat yang aman.

👨‍💻 Pengembang

Dikembangkan dan dirancang khusus untuk optimasi dan digitalisasi administrasi kelengkapan operasional BTPA.

© 2026 Teuku Muhammad Hafidh Rafif
