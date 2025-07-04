Spesifikasi Aplikasi
1. Versi PHP 7.4.9
2. MySql 5.7.31

# Koperasi‑Main
Aplikasi web manajemen koperasi sederhana berbasis PHP yang menyediakan fitur pendaftaran anggota, verifikasi email, login, dan pembayaran simpanan atau saham.
## 🛠️ Fitur Utama

- ✅ **Pendaftaran anggota** dengan verifikasi email otomatis
- 🔐 **Login dan autentikasi** pengguna
- 💰 **Pembayaran simpanan/saham**
- 🔄 **Reset password dan verifikasi ulang email**
- 📄 Struktur modular: HTML partials, assets, dan koneksi DB terpisah
- 🗃️ Database siap pakai: `koperasi.sql`

## 👥 Akses Login
### 🔑 Admin Utama
- **Email**: `koperasikai@gmail.com`  
- **Password**: `koperasikai88`

### 👤 Anggota
- **Email**: `anggota1@gmail.com`  
- **Password**: `anggota1`

---
## 📁 Struktur Direktori

koperasi-main/
├── Login.php
├── Pendaftaran.php
├── ValidasiEmail.php
├── Payment.php
├── LupaPassword.php
├── UlangiVerifikasiEmail.php
├── index.php
├── db/ # Konfigurasi koneksi database
├── forms/ # Formulir pendaftaran & login
├── assets/ # File statis (gambar, CSS, JS)
├── _Page/, _Partial/ # Template halaman & bagian layout
├── koperasi.sql # Skrip database
├── composer.json / lock
├── netlify.toml
└── LICENSE


## 🚀 Cara Instalasi

1. **Clone repository**
   ```bash
   git clone https://github.com/syakillasalsa/koperasi-main.git
   cd koperasi-main
Buat database di XAMPP / phpMyAdmin, misalnya:

sql
Copy
Edit
CREATE DATABASE koperasi_db;
Import file SQL
Buka http://localhost/phpmyadmin
Pilih database koperasi_db
Import file koperasi.sql
Konfigurasi koneksi database
Edit file dalam folder db/ sesuai dengan:

Host: localhost

Username: root
Password: (kosongkan jika default XAMPP)
Database: koperasi_db
Akses Aplikasi di Browser

http://localhost/koperasi-main/Login.php

