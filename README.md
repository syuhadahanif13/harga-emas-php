# Harga-Emas.org Inspired website

**Versi static HTML** dari website harga-emas.org yang sudah dioptimalkan untuk deployment di **Vercel**.

## ✨ Fitur 

- 100% Static (HTML + Tailwind CSS + Vanilla JS + Chart.js)
- Tidak ada PHP lagi → cocok untuk Vercel, Netlify, GitHub Pages
- Tabel harga interaktif (UBS, Antam, Pegadaian)
- Tabs + Quick Buy button
- Modal pembelian dengan perhitungan otomatis
- Grafik harga interaktif (1D/1W/1M/3M/1Y)
- Fully responsive & modern UI
- Dynamic "last updated" time (JavaScript)

## 🚀 Cara Deploy ke Vercel (Super Mudah)

1. Buka [vercel.com](https://vercel.com) dan login
2. Klik **Add New Project**
3. Pilih **Import Git Repository**
4. Pilih repo `syuhadahanif13/harga-emas-php`
5. Klik **Deploy**

Selesai! Website akan otomatis live di `https://harga-emas-php.vercel.app`

## 📁 Struktur File

- `index.html` — File utama (static version)
- `index.php` — Backup versi PHP lama (bisa diabaikan)

## 🔧 Cara Update Harga

Buka `index.html` dan edit array JavaScript di bagian `<script>`:

```js
const ubsPrices = [
    { gram: 1, jual: 2618000, beli: 2380000 },
    ...
];
```

Simpan → push ke GitHub → Vercel otomatis redeploy.

---

Dibuat untuk deployment mudah di Vercel. Semoga bermanfaat! 💛
