# JJJ Delivery Service

Aplikasi pengiriman barang dengan login admin, profile pengguna, estimasi tarif, tracking paket, dan panel admin untuk update status.

## Setup cepat

1. Install dependency:
   npm install
2. Salin file `.env.example` menjadi `.env` dan isi key sesuai kebutuhan.
3. Jalankan aplikasi:
   npm start
4. Buka browser ke http://localhost:3000

## Deploy online ke Render

1. Upload project ini ke repository GitHub baru.
2. Di Render pilih `New` lalu `Blueprint`.
3. Pilih repository tersebut; Render akan membaca `render.yaml`.
4. Isi `GOOGLE_MAPS_API_KEY` saat diminta.
5. Jalankan deploy dan buka URL HTTPS yang diberikan Render.

Render akan menjalankan `npm install`, `npm start`, dan memeriksa `/api/health`.

Catatan: folder `data/` disimpan pada persistent disk Render. Untuk skala besar, migrasikan database ke PostgreSQL.

## Default akun demo

- Admin: admin@jjjdelivery.com / admin123
- Customer: customer@jjjdelivery.com / customer123

## Catatan

- Untuk Google Maps, aktifkan Maps JavaScript API, Places API, dan Directions API di Google Cloud.
- Backend saat ini menggunakan SQLite lokal untuk demo produksi ringan.
- Untuk penggunaan multi-user yang lebih besar, perlu migrasi ke PostgreSQL dan hosting cloud.
