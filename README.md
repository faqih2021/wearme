# WearMe - Online Fashion Store

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

Aplikasi e-commerce berbasis web untuk toko fashion online yang lengkap dengan sistem keranjang belanja, checkout, dan manajemen produk.

## 📋 Deskripsi

WearMe adalah platform e-commerce yang memungkinkan pengguna untuk berbelanja berbagai produk fashion seperti pakaian pria, wanita, dan anak-anak. Aplikasi ini dilengkapi dengan fitur administrasi untuk mengelola produk, pesanan, dan pelanggan.

## ✨ Fitur Utama

### Untuk Pelanggan
- 🛍️ **Browsing Produk**: Jelajahi koleksi fashion untuk pria, wanita, dan anak-anak
- 🔍 **Pencarian Produk**: Cari produk dengan mudah menggunakan fitur search
- 🛒 **Keranjang Belanja**: Tambahkan produk ke keranjang dan kelola pesanan Anda
- 💳 **Checkout System**: Proses checkout yang mudah dan aman
- 📦 **Riwayat Pesanan**: Lihat riwayat pembelian Anda
- ⭐ **Review Produk**: Berikan ulasan dan rating untuk produk
- 👤 **Sistem Login/Register**: Buat akun dan kelola profil Anda

### Untuk Admin
- 📊 **Dashboard Admin**: Panel kontrol untuk mengelola toko
- ➕ **Manajemen Produk**: Tambah, edit, dan hapus produk
- 📋 **Manajemen Pesanan**: Pantau dan kelola pesanan pelanggan
- 👥 **Manajemen User**: Kelola data pelanggan

## 🛠️ Teknologi yang Digunakan

- **Frontend**:
  - HTML5
  - CSS3
  - JavaScript
  
- **Backend**:
  - PHP
  - MySQL Database
  
- **Server**:
  - Apache (XAMPP)

## 📁 Struktur Proyek

```
wearme/
├── HTML/                    # Template HTML
├── src/                     # Asset (gambar, CSS, JS)
├── config.php               # Konfigurasi database
├── index.php                # Halaman utama
├── login.php                # Halaman login
├── Register.php             # Halaman registrasi
├── cart.php                 # Halaman keranjang belanja
├── Checkout.php             # Halaman checkout
├── Order_history.php        # Riwayat pesanan
├── menItem.php              # Produk pria
├── womenItem.php            # Produk wanita
├── kidItems.php             # Produk anak-anak
├── itemDetails.php          # Detail produk
├── search.php               # Pencarian produk
├── About_us.php             # Tentang kami
├── contact-us.php           # Kontak
├── adminLog.php             # Login admin
├── adminHeader.php          # Header admin
├── addItem.php              # Tambah produk (admin)
├── editItem.php             # Edit produk (admin)
├── updateItem.php           # Update produk (admin)
├── addCart.php              # Tambah ke keranjang
├── updateCart.php           # Update keranjang
├── deleteCart.php           # Hapus dari keranjang
├── addReview.php            # Tambah review
├── validateLog.php          # Validasi login
├── adminValidate.php        # Validasi admin
├── enterReg.php             # Proses registrasi
├── logOut.php               # Logout
└── online_fashion.sql       # Database SQL
```

## 🚀 Instalasi dan Setup

### Prerequisites

Pastikan Anda sudah menginstall:
- XAMPP (Apache + MySQL + PHP)
- Web Browser (Chrome, Firefox, dll.)
- Text Editor (VS Code, Sublime, dll.)

### Langkah-langkah Instalasi

1. **Download dan Install XAMPP**
   
   Download dari: [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html)

2. **Clone Repository**
   
   ```bash
   git clone https://github.com/faqih2021/wearme.git
   ```

3. **Pindahkan Project ke htdocs**
   
   Copy folder `wearme` ke direktori:
   ```
   C:\xampp\htdocs\wearme
   ```

4. **Import Database**
   
   - Buka XAMPP Control Panel dan jalankan **Apache** dan **MySQL**
   - Buka browser dan akses: `http://localhost/phpmyadmin`
   - Buat database baru dengan nama `online_fashion`
   - Import file `online_fashion.sql` yang ada di folder project

5. **Konfigurasi Database**
   
   Buka file `config.php` dan sesuaikan dengan konfigurasi Anda:
   ```php
   <?php
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "online_fashion";
   ?>
   ```

6. **Akses Aplikasi**
   
   Buka browser dan akses:
   - **Website**: `http://localhost/wearme`
   - **Admin Panel**: `http://localhost/wearme/adminLog.php`

## 👤 Akun Default

Setelah import database, Anda dapat login dengan akun berikut:

**Admin**
- Email: admin@wearme.com (sesuaikan dengan database)
- Password: admin123 (sesuaikan dengan database)

**User**
- Daftar akun baru melalui halaman Register

## 💡 Cara Penggunaan

### Untuk Pelanggan

1. **Registrasi Akun**
   - Klik tombol "Register" di halaman utama
   - Isi form registrasi dengan data yang valid
   - Klik "Daftar" untuk membuat akun

2. **Login**
   - Masukkan email dan password
   - Klik "Login"

3. **Belanja Produk**
   - Pilih kategori (Men, Women, Kids)
   - Klik produk untuk melihat detail
   - Klik "Add to Cart" untuk menambahkan ke keranjang
   - Atur jumlah barang yang diinginkan

4. **Checkout**
   - Buka keranjang belanja
   - Review pesanan Anda
   - Klik "Checkout" dan isi informasi pengiriman
   - Konfirmasi pesanan

5. **Lihat Riwayat Pesanan**
   - Akses menu "Order History"
   - Lihat detail pesanan Anda

### Untuk Admin

1. **Login Admin**
   - Akses `http://localhost/wearme/adminLog.php`
   - Masukkan kredensial admin

2. **Kelola Produk**
   - Klik "Add Item" untuk menambah produk baru
   - Klik "Edit" untuk mengubah produk
   - Isi form dengan detail produk (nama, harga, gambar, dll.)

3. **Kelola Pesanan**
   - Lihat daftar pesanan pelanggan
   - Update status pesanan

## 📝 Catatan Penting

- Pastikan Apache dan MySQL di XAMPP sudah berjalan sebelum mengakses aplikasi
- Jangan lupa untuk import database `online_fashion.sql` terlebih dahulu
- Sesuaikan konfigurasi database di file `config.php` jika diperlukan
- Untuk production, pastikan menggunakan prepared statements untuk keamanan database

## 🐛 Troubleshooting

**Database Connection Error**
- Pastikan MySQL di XAMPP sudah running
- Cek konfigurasi di `config.php`
- Pastikan database sudah di-import

**Page Not Found**
- Pastikan folder project ada di `htdocs`
- Cek URL yang diakses sudah benar

**Images Not Showing**
- Periksa path gambar di folder `src/`
- Pastikan permission folder sudah benar
