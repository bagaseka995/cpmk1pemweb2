# Resto App - Sistem Informasi Manajemen Restoran

Proyek ini adalah tugas aplikasi berbasis Web (CPMK Pemrograman Web 2) yang dirancang untuk mendigitalisasi proses pemesanan dan pembayaran di sebuah restoran. Aplikasi ini dibangun dengan pendekatan *Object-Oriented Programming* (OOP) menggunakan PHP dan MySQL.

## Fitur Utama
1. **Buku Menu Digital (Akses Publik):**
   - Pelanggan dapat memindai QR Code untuk melihat menu.
   - Dilengkapi dengan fitur **Smart Recommendation** yang menampilkan menu terlaris secara otomatis berdasarkan riwayat pesanan (Best Seller).
   - Pengelompokan menu berdasarkan kategori secara dinamis.
2. **Multi-Role Authentication:**
   - **Admin:** Mengelola data master menu, kategori, dan akun karyawan.
   - **Kasir:** Mengelola status meja, memproses pesanan, dan melakukan transaksi pembayaran.
   - **Pelayan/Dapur:** Memantau monitor dapur (*Kitchen Status*) dari pesanan masuk (Pending) hingga siap disajikan (Served).
3. **Sistem Pembayaran Dinamis:**
   - Mendukung **Split Bill** (Pisah Tagihan) dengan menggunakan *Database Transaction* untuk memecah rincian pesanan tanpa merusak integritas data.
4. **Keamanan:**
   - Enkripsi kata sandi menggunakan `password_hash()`.

## Teknologi yang Digunakan
- **Backend:** PHP 8+ (PDO & OOP)
- **Database:** MySQL / MariaDB
- **Frontend:** HTML5, CSS3 murni (Custom Styling)

## Cara Instalasi
1. *Clone* atau *Download* repositori ini ke dalam folder `htdocs` (jika menggunakan XAMPP).
2. Buat database baru di phpMyAdmin dengan nama `db_resto`.
3. Lakukan *Import* file `db_resto.sql` yang telah disediakan ke dalam database tersebut.
4. Sesuaikan konfigurasi database (username & password) pada file `config/config.php` jika diperlukan.
5. Buka browser dan akses: `http://localhost/cpmk1pemweb2/`
