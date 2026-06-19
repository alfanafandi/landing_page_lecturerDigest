# LectureDigest Landing Page

Halaman web statis minimalis dan premium untuk mempromosikan aplikasi **LectureDigest**, mendemonstrasikan fiturnya secara interaktif, dan menyediakan tautan langsung pengunduhan APK tanpa perlu login.

## Struktur Folder

```
lecturedigest_landing/
├── index.html         # Halaman utama & interaktivitas
├── style.css          # Desain sistem & responsivitas
├── README.md          # Panduan ini
└── app-release.apk    # File APK aplikasi Anda (harus disalin ke sini)
```

## Persiapan Sebelum Deployment

1. Lakukan build APK rilis pada proyek Flutter Anda:
   ```bash
   flutter build apk --release
   ```
2. Salin file APK hasil build tersebut ke dalam folder ini. File APK terletak di:
   `c:\laragon\www\lecturer_digest\build\app\outputs\flutter-apk\app-release.apk`
3. Tempel file tersebut ke dalam folder `lecturedigest_landing/` ini dan pastikan namanya tetap `app-release.apk`.

## Uji Coba Lokal

Anda dapat menjalankan halaman ini secara lokal menggunakan ekstensi Live Server (di VS Code) atau menggunakan python server di terminal:
```bash
python -m http.server 8000
```
Lalu buka `http://localhost:8000` di browser Anda.

## Cara Deployment ke Vercel (Gratis & Sangat Cepat)

1. Masuk ke folder landing page ini di terminal Anda:
   ```bash
   cd lecturedigest_landing
   ```
2. Inisialisasi Git baru di dalam folder ini (agar terpisah dari git utama):
   ```bash
   git init
   git add .
   git commit -m "Inisialisasi landing page rilis"
   ```
3. Buat repositori baru di GitHub (misal bernama `lecturedigest-landing`) secara **Public**, lalu hubungkan dan push kode Anda ke sana:
   ```bash
   git remote add origin https://github.com/username/lecturedigest-landing.git
   git branch -M main
   git push -u origin main
   ```
4. Buka [Vercel Dashboard](https://vercel.com/dashboard), buat proyek baru, lalu hubungkan dengan repositori `lecturedigest-landing` yang baru saja Anda buat.
5. Klik **Deploy**. Selesai! Aplikasi Anda beserta APK-nya sekarang online dan siap dinilai juri.
