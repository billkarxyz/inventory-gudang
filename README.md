# Inventory Gudang

Sistem pencatatan stok barang gudang — sederhana, tanpa server, tanpa instalasi.

## Fitur

- **Dashboard** — total jenis barang, total stok, nilai stok (harga × stok), dan jumlah barang yang stoknya menipis.
- **Daftar barang** — tabel dengan kode/SKU, nama, kategori, lokasi rak, satuan, harga, stok, dan stok minimum. Bisa dicari dan difilter per kategori. Baris yang stoknya menipis (stok ≤ stok minimum) ditandai merah.
- **Tambah / edit / hapus barang** — kode barang terisi otomatis (BRG-001, BRG-002, ...) tapi bisa diubah.
- **Barang masuk & keluar** — pilih barang, jumlah, dan catatan; stok langsung berubah dan tercatat di riwayat.
- **Riwayat pergerakan** — semua barang masuk/keluar beserta tanggal, jumlah, stok setelahnya, dan catatan.
- **Export CSV** — daftar barang dan riwayat bisa diunduh sebagai file CSV (bisa dibuka di Excel / Google Sheets).
- **Data tersimpan lokal** — semua data tersimpan di browser (localStorage), jadi tetap ada setelah halaman ditutup dan dibuka lagi. Ada tombol **Muat Data Contoh** dan **Hapus Semua Data**.

## Cara memakai

Tidak perlu instalasi atau server:

1. Unduh / clone repo ini.
2. Buka file `index.html` di browser (klik dua kali).
3. Saat pertama dibuka, data contoh (10 barang gudang) langsung dimuat supaya bisa langsung dicoba.

Alternatif: aktifkan **GitHub Pages** di repo ini (Settings → Pages → Branch `main`, folder `/ (root)`) supaya aplikasinya bisa dibuka lewat link.

## Teknologi

- HTML + CSS + JavaScript murni (tanpa framework, tanpa dependensi).
- Satu file `index.html` — semua tampilan dan logika ada di dalamnya.
- Penyimpanan: `localStorage` browser.
