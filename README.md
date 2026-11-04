# tokoku — online shop (HTML + CSS saja)

Website toko online statis berbahasa Indonesia, dibuat **hanya dengan HTML dan CSS**. Tidak ada JavaScript, framework, build tool, atau dependensi npm.

## Cara membuka

Buka `index.html` langsung di browser, atau jalankan server statis:

```bash
python -m http.server 8123
```

Lalu buka `http://127.0.0.1:8123/index.html`.

## Struktur file

```
index.html            Halaman utama: hero, katalog, promo, keunggulan, newsletter, footer
checkout.html         Halaman checkout + ringkasan pesanan (statis)
assets/css/style.css  Semua styling: token warna, komponen, filter CSS, responsive
assets/img/*.svg      10 ilustrasi produk (SVG lokal, tanpa internet)
```

## Fitur

- Katalog 10 produk dengan ilustrasi lokal dan layout responsif (4 / 3 / 2 / 1 kolom).
- **Filter kategori berfungsi tanpa JavaScript**, memakai radio input dan selector CSS `:has()`.
- Halaman checkout dengan form pengiriman, pilihan ongkir, metode pembayaran, dan ringkasan pesanan.
- Bagian promo, keunggulan toko, newsletter, dan footer lengkap.
- Efek hover, transisi halus, serta dukungan `prefers-reduced-motion`.

## Batasan (karena tanpa JavaScript)

- Keranjang tidak menghitung otomatis; halaman checkout berisi contoh pesanan statis.
- Tombol "Berlangganan", "Buat pesanan", dan pilihan kode promo hanya tampilan.
- Pencarian dan pengurutan produk tidak tersedia.

Semua itu butuh JavaScript atau backend. Struktur HTML/CSS ini sudah siap dipasangi logika tersebut nanti.
