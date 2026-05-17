# Produktografi — Portfolio Website

Situs portofolio fotografi ringan berbasis HTML+Tailwind.

## Fitur utama
- Galeri 2x3 dengan efek grayscale → warna saat hover/touch/scroll.
- Lightbox (klik gambar untuk zoom) responsif di desktop & mobile.
- Auto slider yang menggunakan gambar galeri.
- Tombol cepat: WhatsApp (chat langsung), Instagram, Email.
- Floating `BOOK NOW` terhubung ke WhatsApp.

## Quick start
1. Buka folder proyek (`w:/produktografi`) di VS Code.
2. Mulai server lokal untuk preview:

Dengan Python (buka terminal di folder proyek):

```bash
python -m http.server 5500
```
Buka: http://127.0.0.1:5500/index.html

Atau gunakan VS Code Live Server extension (klik "Go Live").

## Cara kustomisasi cepat
- Ubah nomor WhatsApp: cari `wa.me/` di `index.html` dan ganti nomor (format E.164 tanpa +, contoh `62821...`).
- Ubah link Instagram: cari `https://www.instagram.com/produktografi/`.
- Ganti logo: cari tag `<img` dengan `logo_` atau `logob_` di `index.html` dan ganti `src` ke URL Cloudinary Anda.
- Ganti gambar galeri/slider: edit `src` atribut di elemen `<img>` dalam bagian `#portfolio` atau `.slider-track`.

## Perilaku mobile
- Sentuhan (`touchstart`) pada kartu galeri akan menonaktifkan grayscale sementara dan membuka lightbox saat diklik.
- Scroll observer menandai gambar yang masuk area terlihat untuk menampilkan warna.

## Pengujian & debugging
- Jika lightbox atau efek tidak bekerja, buka DevTools → Console untuk melihat error JavaScript.
- Untuk memastikan perubahan gambar segera terlihat, hard-reload browser atau bersihkan cache.

## Lanjutkan
- Mau saya commit perubahan ke git? (saya bisa membuat commit message dan branch.)

---
Created and maintained by the Produktografi project files in this workspace.