💨 Vape Store V1 - Database Management System

Proyek ini adalah implementasi database SQL untuk pengelolaan toko vape (Vape Store). Database ini mencakup manajemen inventaris, data karyawan, shift kerja, hingga sistem transaksi yang dilengkapi dengan fitur kalkulasi pajak dan pelaporan omzet.

👥 Profil Kelompok

Dokumentasi ini disusun oleh anggota kelompok berikut:

- Iqbal Hadi Widyadana (NIM: 250119011)
- Fauzan Fathoni Khoirul Huda (NIM: 250119007)

🛠️ Struktur Database

Database vape_storeV1 terdiri dari beberapa tabel utama yang saling berelasi:

Tabel SDM: karyawan, operator (akun sistem), dan kasir (lokasi pos).

Tabel Operasional: shift dan jadwal (manajemen waktu kerja).

Tabel Inventaris: items (pendataan stok dan harga barang).

Tabel Transaksi: transaksi (header penjualan) dan transaksi_detail (rincian item yang terjual).

🚀 Fitur Query Utama

Berikut adalah fitur-fitur query yang diimplementasikan berdasarkan materi ORDER BY hingga JOIN:

1. Manajemen Inventaris

Monitoring Stok: Menggunakan HAVING untuk mendeteksi barang dengan stok kritis (di bawah 20).

Pencarian Produk: Menggunakan operator LIKE untuk mencari kategori produk tertentu (misal: 'Liquid').

Analisis Harga: Menampilkan harga termahal menggunakan ORDER BY DESC dan rata-rata harga menggunakan fungsi AVG.

2. Sistem Transaksi & Keuangan

Kalkulasi Otomatis: Menghitung estimasi PPN 10% dan harga total setelah pajak menggunakan Alias dan operasi aritmatika.

Laporan Omzet: Menggunakan GROUP BY dan SUM untuk menghitung total pendapatan per titik kasir.

Detail Transaksi: Penggunaan JOIN multi-tabel untuk menampilkan struk belanja yang lengkap (Nama Kasir, Nama Barang, dan Subtotal).

3. Audit & Relasi Data

Audit Akun: Menggunakan LEFT JOIN untuk mengidentifikasi karyawan yang belum memiliki akun operator sistem.

Relasi User: Menggunakan RIGHT JOIN dan UNION (Simulasi Full Join) untuk memetakan hubungan antara data personal karyawan dengan kredensial sistem.

📝 Cara Menjalankan

Pastikan Anda memiliki MySQL Server/XAMPP yang aktif.

Salin seluruh konten dari file vape_store-UAS_DONE.sql.

Jalankan query di MySQL Workbench atau phpMyAdmin.

Database vape_store-UAS-DONE akan otomatis terbuat beserta seluruh contoh datanya.

Proyek ini dikembangkan untuk memenuhi tugas mata kuliah Pemrograman Basis Data.
