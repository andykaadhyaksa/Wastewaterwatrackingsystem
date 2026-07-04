# IPAL Checker

Aplikasi web single-file untuk mengecek kesesuaian desain IPAL terhadap Permen LH No. 11/2025.

## Cara deploy ke GitHub Pages

1. Buat repository baru di GitHub (misal: `ipal-checker`).
2. Upload semua file di folder ini (index.html, favicon.ico, manifest.json, folder icons/) ke root repository tersebut — pastikan strukturnya persis seperti di folder ini (jangan ubah nama file/folder).
3. Buka **Settings → Pages** di repository.
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit, lalu buka URL yang muncul (biasanya `https://<username>.github.io/<nama-repo>/`).
6. Buka URL tersebut di Chrome, lalu bookmark halaman tersebut — ikon aplikasi (pipa air) akan otomatis muncul di bookmark/tab karena favicon & manifest sudah disertakan.

## Perbaikan pada versi ini

1. **Logo** — ikon di header aplikasi kini menggunakan logo yang sama persis dengan file `Logo_IPAL_Checker.png` yang dikirim.
2. **Favicon / ikon bookmark** — ditambahkan `favicon.ico`, ikon PNG berbagai ukuran (16px–512px) di folder `icons/`, dan `manifest.json` sehingga logo muncul di tab browser dan saat di-bookmark di Chrome, termasuk saat di-hosting di GitHub Pages.
3. **Data tidak hilang saat pindah menu** — semua input (Debit, BOD, COD, MLVSS, dimensi unit proses, dsb.) sekarang otomatis tersimpan setiap kali:
   - Anda mengetik di kolom manapun (bukan hanya saat keluar dari kolom/blur).
   - Anda berpindah menu (Dashboard, Data IPAL, Perhitungan, Hasil, dst).
   - Selain itu ditambahkan **autosave cadangan** ke penyimpanan browser (localStorage): jika tab tidak sengaja tertutup atau di-refresh, aplikasi akan menawarkan untuk memulihkan data yang belum sempat disimpan saat dibuka kembali.

## File dalam paket ini

```
index.html          -> aplikasi utama (buka file ini langsung di browser, atau hosting via GitHub Pages)
favicon.ico          -> ikon browser tab
manifest.json         -> metadata PWA/bookmark icon
icons/                -> ikon PNG berbagai resolusi (16–512px)
README.md            -> file ini
```
