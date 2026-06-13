# Harga-Emas.org Clone

Website clone sederhana dari [harga-emas.org](https://harga-emas.org) dibuat dengan **pure PHP** + **Tailwind CSS** (Play CDN) + **Chart.js**.

## ✨ Fitur

- **Navbar responsif** dengan menu smooth scroll + mobile hamburger
- **Spot Harga** USD & IDR real-time style cards
- **Tabel Harga Emas Interaktif**:
  - Tabs: UBS Gold 99.99% • Antam • Pegadaian
  - Harga Jual & Beli per gram (data akurat dari screenshot Juni 2026)
  - Tombol "Beli" cepat di setiap baris
- **Grafik Harga** interaktif dengan Chart.js (1D, 1W, 1M, 3M, 1Y)
- **Modal Pembelian** simulasi lengkap dengan perhitungan total otomatis
- **Promo Pluang** section yang menarik
- **Fully responsive** & modern UI dengan gold accent color
- **Pure PHP** – data harga mudah di-update di bagian atas file `index.php`
- Tidak perlu database, composer, atau framework

## 🚀 Cara Menjalankan

### Lokal (paling mudah)

```bash
# Masuk ke folder project
cd harga-emas-php

# Jalankan built-in PHP server
php -S localhost:8000
```

Buka browser: **http://localhost:8000**

### Deploy ke Hosting PHP Biasa

Upload seluruh folder ke hosting (cPanel, InfinityFree, Hostinger, dll). Tidak perlu konfigurasi khusus.

### Deploy ke Vercel / Netlify (opsional)

Karena pure PHP, lebih baik pakai hosting PHP tradisional. Untuk Vercel bisa pakai adapter PHP jika mau.

## 📝 Cara Update Harga

Buka `index.php` dan edit array PHP di bagian atas:

```php
$ubs_prices = [
    ['gram' => 1, 'jual' => 2618000, 'beli' => 2380000],
    // ...
];
```

Ubah sesuai data terbaru. Simpan → refresh browser.

## 🛠 Teknologi

- PHP 8+ (hanya untuk tanggal & data rendering)
- Tailwind CSS via CDN (Play)
- Chart.js via CDN
- Font Awesome 6
- Vanilla JavaScript (tidak ada framework)

## 📸 Preview

Website ini meniru tampilan asli harga-emas.org dengan:
- Warna gold/amber yang elegan
- Tabel modern dengan hover effect
- Interaksi yang responsif (tabs, modal, chart period switch)
- Fokus pada kemudahan penggunaan

---

**Catatan**: Ini adalah proyek pembelajaran / demo. Bukan situs resmi. Data harga diambil dari tangkapan layar Juni 2026 dan bersifat simulasi.

Dibuat untuk Arjun Prayudha / Zeps — semoga bermanfaat untuk TA atau project lainnya! 💛
