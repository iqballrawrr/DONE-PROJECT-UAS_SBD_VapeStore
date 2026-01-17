<p align="center">
  <img src="https://lh3.googleusercontent.com/d/1-TrhdCX8Geg0MPz6wW44Gst2bRhawRC3" width="300" alt="TRPL Logo">
</p>

<h1 align="center">💨 Vape Store V1</h1>

<p align="center">
  <b>Database Management System untuk Pengelolaan Toko Vape</b><br>
  Proyek Mata Kuliah <i>Pemrograman Basis Data</i>
</p>

---

## 📌 Deskripsi Proyek
**Vape Store V1** adalah implementasi **Database SQL** yang dirancang untuk mengelola operasional toko vape secara terstruktur dan efisien.  
Database ini mencakup pengelolaan **inventaris barang**, **data karyawan**, **jadwal & shift kerja**, serta **sistem transaksi penjualan** yang dilengkapi dengan **perhitungan pajak dan laporan omzet**.

Proyek ini dibuat sebagai bentuk penerapan materi **query SQL lanjutan**, mulai dari `ORDER BY`, `GROUP BY`, `HAVING`, hingga `JOIN`.

---

## 👥 Profil Kelompok
Dokumentasi dan pengembangan database ini disusun oleh:

- **Iqbal Hadi Widyadana**  
  🆔 NIM: 250119011  

- **Fauzan Fathoni Khoirul Huda**  
  🆔 NIM: 250119007  

---

## 🛠️ Struktur Database
Database **`vape_storeV1`** terdiri dari beberapa tabel utama yang saling berelasi:

### 🔹 Tabel SDM
- `karyawan` — data pegawai  
- `operator` — akun sistem  
- `kasir` — lokasi atau titik kasir  

### 🔹 Tabel Operasional
- `shift` — jam kerja  
- `jadwal` — penjadwalan karyawan  

### 🔹 Tabel Inventaris
- `items` — data stok barang, kategori, dan harga  

### 🔹 Tabel Transaksi
- `transaksi` — header penjualan  
- `transaksi_detail` — detail item yang terjual  

---

## 🚀 Fitur Query Utama
Query dibuat berdasarkan materi **ORDER BY hingga JOIN**, dengan fitur sebagai berikut:

### 📦 Manajemen Inventaris
- **Monitoring Stok**  
  Menggunakan `HAVING` untuk mendeteksi stok kritis (stok < 20).
- **Pencarian Produk**  
  Menggunakan `LIKE` untuk mencari kategori tertentu (contoh: *Liquid*).
- **Analisis Harga**  
  - Harga tertinggi (`ORDER BY DESC`)  
  - Rata-rata harga (`AVG`)

---

### 💰 Sistem Transaksi & Keuangan
- **Kalkulasi Otomatis**  
  Perhitungan PPN 10% dan total harga menggunakan *alias* dan operasi aritmatika.
- **Laporan Omzet**  
  `GROUP BY` dan `SUM` untuk menghitung total pendapatan per kasir.
- **Detail Transaksi Lengkap**  
  `JOIN` multi-tabel untuk menampilkan struk belanja (Kasir, Barang, Subtotal).

---

### 🔍 Audit & Relasi Data
- **Audit Akun Operator**  
  `LEFT JOIN` untuk mendeteksi karyawan yang belum memiliki akun sistem.
- **Relasi Data User**  
  `RIGHT JOIN` dan `UNION` (simulasi *FULL JOIN*) untuk memetakan data karyawan dan akun login.

---

## 📝 Cara Menjalankan
1. Pastikan **MySQL Server / XAMPP** dalam keadaan aktif.
2. Salin seluruh isi file:
