# TUGAS 1 PENGEMBANGAN APLIKASI

## Fitur

### Pembeli:
- Melihat daftar roti yang tersedia (stok)

- Memesan roti sesuai keinginan

- Melihat total harga belanja

- Transaksi disimpan ke riwayat pembelian

### Penjual:
- Menambahkan produk roti ke stok

- Melihat stok roti

- Melihat total pemasukan

- Melihat riwayat pembelian dan data pembeli

## fitur tambahan 
- riwayat pembelian otomatis tersimpan
- rekap total pemasukan dari hasil transaksi
- validasi input angka

## optimisasi:

- Eliminasi duplikasi kode, penggunaan fungsi input_int() untuk input angka.

- Perbaikan efisiensi pencarian produk: menggunakan produk[produk["Nama"].str.lower() == nama_roti.lower()] ketimbang loop manual.

- Pemrosesan keranjang dan stok lebih aman dan efisien.

- Struktur fungsi dipisahkan dengan lebih modular agar mudah diuji/diubah.

- Penulisan ulang logika menu utama agar lebih ringkas dan mudah dibaca.

# TUGAS 2 DOKUMENTASI TEKNIS

## Dokumen Spesifikasi Sistem
Aplikasi ini merupakan simulasi toko roti berbasis Python menggunakan antarmuka baris perintah (CLI). Dibuat untuk keperluan pembelajaran atau tugas praktikum. Sistem terdiri dari dua peran utama:

Penjual: mengelola produk, melihat pemasukan, dan riwayat transaksi.

Pembeli: melihat daftar roti, memesan, dan membayar.

## Code Documentation yang lengkap
Sudah tersedia komentar dan struktur kode terorganisir per bagian: inisialisasi, fungsi penjual, pembeli, dan menu utama.

## Diagram Alur Kerja dan Arsitektur

A. Program dimulai
B. Menampilkan menu utama:
   
   1. Login sebagai Pembeli
   2. Login sebagai Penjual
   3. Keluar

C. Jika pengguna memilih Pembeli:
   1. Input nama pembeli
   
   2. Menampilkan menu pembeli:
      
        1. Lihat stok roti
        2. Beli roti
        3. Selesai dan Bayar
   
   3. Jika memilih lihat stok → tampilkan daftar stok
   
   4. Jika memilih beli roti:
      
        - Input nama roti dan jumlah
        - Cek apakah stok cukup
        - Jika cukup → masukkan ke keranjang
        - Jika tidak → tampilkan pesan stok tidak cukup
   
   5. Jika memilih selesai dan bayar:
      
        - Tampilkan ringkasan belanja
        - Tambahkan pemasukan
        - Simpan ke riwayat pembelian

D. Jika pengguna memilih Penjual:
   
   1. Menampilkan menu penjual:
      
        1. Tambah roti ke stok
        2. Lihat stok roti
        3. Lihat total pemasukan
        4. Lihat riwayat pembelian
        5. Kembali ke menu utama
   
   2. Penjual bisa menambahkan roti (input nama, harga, stok)
   
   3. Bisa melihat stok, pemasukan, dan transaksi.

E. Jika memilih keluar:
   - Program akan berhenti dan menampilkan pesan terima kasih

F. Program selesai

# TUGAS 3 USER MANUAL

## Panduan instalasi
- buka google colab
  
- buat notebook baru
  
- salin dan tempel kode aplikasi
  
- jalankan kodenya dengan klik run

##  Tutorial Penggunaan Aplikasi

Pada menu utama akan muncul beberapa pilihan login

### Sebagai Pembeli:

- Pilih menu 1

- Masukkan nama pembeli

- Pilih “Beli Roti” dan masukkan nama roti & jumlah

- Lanjutkan hingga selesai, lalu pilih “Selesai dan Bayar”

### Sebagai Penjual:

- Pilih menu 2

- Tambah produk, cek stok, cek pemasukan, atau lihat riwayat pembelian

- jika sudah menambahkan satu produk akan ditanya apakah ingin menambah produk lainnya atau tidak

lalu ketik 3 untuk keluar

## FAQ dan Troubleshooting
Q: Tidak bisa input angka?

A: Pastikan hanya mengetik angka, bukan huruf atau simbol

Q: Data stok hilang setelah keluar?

A: Aplikasi ini belum menyimpan ke file. Gunakan fitur backup (fitur tambahan)

#  TUGAS 4 PENGUJIAN DAN EVALUASI

## Pengujian Fitur

Setiap fitur dalam aplikasi telah diuji secara manual:

- Saat menambah produk, sistem berhasil menyimpan nama, harga, dan jumlah stok roti.

- Saat membeli roti, sistem mengecek apakah stok mencukupi sebelum memproses pembelian.

- Jika nama roti salah atau stok tidak mencukupi, sistem menampilkan pesan kesalahan yang jelas.

- Setelah pembelian selesai, sistem mencatat riwayat pembelian dan menambahkan total pemasukan.

## Pengujian Validasi

- Input angka yang salah (misalnya huruf atau simbol) akan ditolak dengan pesan peringatan.

- Jika pembeli mencoba membeli roti yang tidak tersedia atau tidak ada stok, aplikasi akan menolak transaksi tersebut.
  
## Analisis Kinerja dan Optimasi

- Aplikasi berjalan lancar untuk input skala kecil hingga menengah.

- Tidak ditemukan bug besar saat pengujian.

- Optimasi dilakukan pada bagian input (validasi angka), penggunaan fungsi reusable untuk menghindari duplikasi kode, serta struktur menu yang lebih modular agar mudah dikembangkan.
