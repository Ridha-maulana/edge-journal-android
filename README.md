# Edge Journal — Android (Capacitor)

Pembungkus aplikasi Android untuk Edge Journal. Aplikasi memuat web Edge Journal dari
`https://ridha-maulana.github.io/edge-journal-v3.0.0/` (repositori web terpisah), jadi
pembaruan web otomatis ikut tanpa membuat APK baru. Jika APK bermasalah, versi web tetap berjalan.

## Isi
- `capacitor.config.json` — alamat web yang dimuat, warna, splash
- `package.json` — paket Capacitor (Android, Filesystem, Share, Haptics, Splash Screen)
- `assets/` — ikon dan splash sumber
- `splash-res/` — ikon splash Android bersudut tumpul (vektor), disalin ke proyek saat build
- `www/` — halaman cadangan (tidak dipakai saat alamat web aktif)
- `debug.keystore` — kunci penanda tetap supaya APK baru bisa memperbarui APK lama
- `build-apk.yml` — salin ke `.github/workflows/build-apk.yml` (dibuat manual sekali)

## Hasil
APK muncul di halaman **Releases** repositori ini setiap kali Action "Build APK" selesai.
