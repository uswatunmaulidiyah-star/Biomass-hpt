# Biomass HPT Calculator

Kalkulator HPT biomassa dengan Biomass Master Data yang bisa diubah (tambah, edit, hapus), impor dan ekspor Excel, serta riwayat perhitungan.

Rumus: `HPT = 70 × (Setting GCV ÷ 6.322) × Kurs USD × 1,2`

## Cara memasang di GitHub Pages (gratis)

1. Buat akun gratis di https://github.com lalu masuk.
2. Klik **New repository**. Beri nama, misalnya `biomass-hpt`. Pilih **Public** (GitHub Pages gratis memerlukan repository publik). Klik **Create repository**.
3. Di halaman repository, klik **uploading an existing file** (atau **Add file > Upload files**).
4. Seret file `index.html` dan `README.md` ke halaman itu, lalu klik **Commit changes**.
5. Buka **Settings > Pages**. Pada **Build and deployment**, pilih **Source: Deploy from a branch**. Pilih branch **main** dan folder **/ (root)**, lalu klik **Save**.
6. Tunggu 1 sampai 2 menit. Alamat situs akan tampil di halaman yang sama:
   `https://NAMA-AKUN-ANDA.github.io/biomass-hpt/`

## Memperbarui aplikasi

Buka repository, klik `index.html`, klik ikon pensil atau pilih **Add file > Upload files**, unggah file baru dengan nama yang sama, lalu **Commit changes**. Situs diperbarui dalam beberapa menit.

## Tentang data

- Data master, kurs terakhir, dan riwayat perhitungan disimpan di localStorage browser. Data tidak dikirim ke GitHub dan tidak terlihat oleh orang lain.
- Setiap browser dan perangkat punya data sendiri. Untuk memindahkan atau mencadangkan data, pakai **Export Excel** dan **Import Excel** di tab Biomass Master Data.
- Membersihkan data situs di browser akan menghapus data master. Lakukan Export Excel secara berkala.
- Karena repository publik, kode aplikasi bisa dilihat siapa saja. Jangan menaruh data rahasia di dalam file `index.html`.

## Catatan teknis

Aplikasi ini satu file HTML tanpa proses build. Font dan library Excel (SheetJS) dimuat dari CDN, jadi perangkat pengguna memerlukan koneksi internet saat membuka halaman.
