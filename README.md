# Kas Kelas 3B — Agustus 2026 s.d. Juni 2027

Aplikasi web satu-file (`index_clean-2.html`) untuk mencatat dan merekap kas kelas serta iuran TIK. Tidak butuh server atau instalasi — cukup dibuka lewat browser.

## Cara Pakai

1. Buka file `index_clean-2.html` di browser (Chrome/Safari, desktop maupun HP).
2. Semua data otomatis tersimpan di browser (localStorage) setiap kali ada perubahan — tidak perlu tombol "Simpan" terpisah.
3. Karena datanya tersimpan di browser, buka file ini dari **perangkat/browser yang sama** setiap kali supaya data tidak hilang atau tidak "ganda" antar device.

## Dua Mode Pembukuan

Ada tombol pindah mode di bagian atas:

- **📒 Kas Bulanan** — pencatatan kas rutin kelas.
- **💻 TIK** — pencatatan iuran TIK, terpisah dari kas bulanan (data, saldo, dan riwayatnya sendiri-sendiri).

### Mode Kas Bulanan
- **Rekap** — ringkasan total masuk, keluar, dan saldo per bulan (Agustus 2026 – Juni 2027). KPI card di atas bisa diklik untuk lompat ke halaman terkait (Pemasukan, Pengeluaran, Kas per Bulan, Data Siswa).
- **Data Siswa** — daftar siswa & status bayar per bulan (centang otomatis berdasarkan input pemasukan).
- **Input Pemasukan / Pengeluaran** — form catat transaksi.
- **Kas per Bulan** — rincian per bulan.
- **Cetak** — tombol 🖨️ Cetak punya beberapa pilihan: Cetak Semua, Cetak Rekap, Cetak Bulanan, Cetak Rincian (semua dioptimalkan untuk kertas A4).
- **Export ke Excel** — unduh seluruh data kas sebagai file `.xlsx`.

### Mode TIK
- Struktur sama seperti Kas Bulanan (Rekap, Data Siswa, Input Pemasukan, Input Pengeluaran) tapi khusus iuran TIK, dengan rentang bulan Agustus 2026 – Mei 2027.
- Tombol Cetak (Cetak Semua / Cetak Rekap / Cetak Rincian) dan Export ke Excel tersedia terpisah dari mode Kas.

## Menambah / Menghapus Siswa

Data siswa disinkronkan otomatis antara mode Kas dan TIK saat pertama kali dibuat. Untuk menambah atau menghapus siswa, gunakan tombol **＋ Tambah Siswa** / ikon 🗑️ di halaman Data Siswa pada masing-masing mode.

## Backup Data

Karena data tersimpan lokal di browser (bukan di cloud), disarankan rutin melakukan **Export ke Excel** sebagai cadangan, terutama sebelum membersihkan cache/data browser atau ganti perangkat.

## Riwayat Perbaikan

- Header ganda saat mencetak Rekap TIK — diperbaiki.
- Tabel Data Siswa pada cetak Rekap Kas yang kolomnya tidak rapi — diperbaiki (kini menyesuaikan lebar halaman A4 tanpa terpotong).
- Kolom "Keterangan" pada tabel Ringkasan TIK — dirapikan jadi rata tengah.
- Gaya tombol "Export ke Excel" (outline hijau tua, background putih) dan "Cetak" (outline hijau tua, background hijau muda) diseragamkan.
- Kotak KPI "Total Pemasukan" pada mode TIK yang salah arah ke Data Siswa — diperbaiki, kini menuju Daftar Pemasukan TIK.
