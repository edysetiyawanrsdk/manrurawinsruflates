# ManruraPod - Aplikasi Manajemen Penilaian

Aplikasi ManruraPod adalah sistem manajemen penilaian untuk ruangan/unit yang memungkinkan:
- Penilaian mandiri (self-assessment) oleh perwakilan ruangan
- Evaluasi oleh tim evaluator
- Pengelolaan standar dan item penilaian
- Dashboard statistik dan laporan

## Teknologi yang Digunakan

- **Frontend**: React.js, TailwindCSS, shadcn/ui
- **Backend**: Express.js (Node.js)
- **Database**: PostgreSQL (Neon Database - serverless)
- **ORM**: Drizzle ORM
- **Autentikasi**: Passport.js (otentikasi lokal)

## Fitur Utama

- Multi-user dengan tiga peran: admin, user_room, dan evaluator
- Manajemen ruangan/unit
- Manajemen standar dan item penilaian
- Sistem penilaian mandiri dengan bukti pendukung
- Evaluasi oleh tim penilai
- Dashboard statistik
- Laporan hasil penilaian

## Cara Menjalankan Aplikasi

### Prasyarat

- Node.js 18 atau lebih baru
- PostgreSQL database (atau Neon database URL)

### Instalasi

1. Clone repository ini
   ```
   git clone https://github.com/yourusername/manrurawinsruflates.git
   cd manrurawinsruflates
   ```

2. Install dependensi
   ```
   npm install
   ```

3. Siapkan variabel lingkungan
   Buat file `.env` dengan konten:
   ```
   DATABASE_URL=postgres://username:password@hostname:port/database
   ```

4. Jalankan aplikasi dalam mode pengembangan
   ```
   npm run dev
   ```

### Build untuk Production

```
npm run build
npm start
```

## Deployment di Vercel

Aplikasi ini sudah dikonfigurasi untuk deployment di Vercel. Anda dapat menggunakan tombol dibawah untuk deploy secara langsung:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fyourusername%2Fmanrurawinsruflates)

### Variabel Lingkungan di Vercel

- `DATABASE_URL`: URL koneksi PostgreSQL (Neon database)
- `NODE_ENV`: Diatur ke `production` untuk mode produksi

## Lisensi

MIT
