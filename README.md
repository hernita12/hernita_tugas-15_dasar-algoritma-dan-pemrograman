##🥐 Aplikasi Toko Roti Sederhana
Aplikasi ini merupakan simulasi toko roti berbasis Python menggunakan antarmuka baris perintah (CLI). Dibuat untuk keperluan pembelajaran atau tugas praktikum.

##📌 Fitur
#👤 Pembeli:
- Melihat daftar roti yang tersedia (stok)

- Memesan roti sesuai jumlah

- Melihat total harga belanja

- Transaksi disimpan ke riwayat pembelian

#🧑‍💼 Penjual:
- Menambahkan produk roti ke stok

- Melihat stok roti

- Melihat total pemasukan

- Melihat riwayat pembelian dan data pembeli


#optimasi:
| Area             | Perbaikan                                                                   |
| ---------------- | --------------------------------------------------------------------------- |
| Struktur fungsi  | Fungsi lebih modular (dipisah dan ringkas)                                  |
| Perulangan       | Hindari `while True` tak perlu, gunakan loop yang efisien                   |
| Global variable  | Hindari penggunaan `global` (diganti lewat parameter & return)              |
| Pengolahan data  | Gunakan dictionary lebih rapi, dan `pandas` digunakan hanya saat dibutuhkan |
| Validasi input   | Menambahkan pengecekan input dan error handling ringan                      |
| Pengulangan kode | Bagian seperti `lihat_stok()` tidak dipanggil dua kali                      |
