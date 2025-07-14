# Aplikasi Pemesanan Makanan - FoodOrderku 🍔
Aplikasi web sederhana untuk memesan makanan secara online.

## Fitur
- Login user & admin
- Daftar menu makanan
- Pemesanan dan laporan
- Backup data ke CSV

## Cara Install
1. Clone repo ini
2. Jalankan XAMPP → Aktifkan Apache & MySQL
3. Import database dari `database/foodorder_db.sql`
4. Akses `localhost/foodorderku`

## Login
- Admin: `admin` / `admin`
- User: `user` / `user`

/foodorderku
├── index.php
├── login.php
├── menu.php
├── order.php
├── admin/
│   ├── dashboard.php
│   └── kelola_menu.php
├── assets/
│   ├── css/
│   └── img/
├── backup/
├── config/
│   └── koneksi.php
├── database/
│   └── foodorder_db.sql
└── README.md
