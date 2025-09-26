# IT Application Support Test

Selamat — ini adalah repository berisi materi tes untuk posisi **IT Application Support**.

## Isi repository
- `IT Application Support Test.docx` — dokumen soal tes (API & Database Integration - Node.js + PostgreSQL/MySQL).
- `README.md` — file ini, berisi instruksi singkat.
- `.gitignore` — saran file yang diabaikan (node_modules, .env).
- `LICENSE` — lisensi MIT singkat.

## Tujuan Tes
Kandidat diminta untuk membuat sebuah project **Node.js + Express** yang mengimplementasikan API CRUD terhadap tabel `employees` pada database relasional (PostgreSQL atau MySQL).

## Instruksi untuk kandidat (singkat)
1. Buat project Node.js + Express.
2. Gunakan PostgreSQL **atau** MySQL.
3. Implementasikan endpoint:
   - `GET /employees` → semua karyawan
   - `GET /employees/:id` → detail karyawan
   - `POST /employees` → tambah karyawan
   - `PUT /employees/:id` → update karyawan
   - `DELETE /employees/:id` → hapus karyawan
4. Sertakan `README.md` di repo kandidat yang menjelaskan cara:
   - instal dependensi (`npm install`)
   - menjalankan aplikasi (`npm start` atau `node index.js`)
   - konfigurasi environment (contoh `DATABASE_URL` atau file `.env`)
5. Sertakan SQL untuk membuat tabel `employees` atau migration.
6. Push hasil ke **GitHub (public)** dan kirimkan link repo ke tim recruitment.

## Contoh struktur tabel `employees`
```sql
CREATE TABLE employees (
  id SERIAL PRIMARY KEY,
  name VARCHAR(255) NOT NULL,
  email VARCHAR(255) UNIQUE NOT NULL,
  position VARCHAR(100),
  salary NUMERIC,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

## Penilaian singkat
- Kebenaran API dan operasi CRUD
- Dokumentasi (README)
- Struktur project dan kualitas kode
- Cara menjalankan (klaritas instruksi)
- Bonus: test sederhana (unit/integration) atau Postman collection

## Kontak
Jika ada pertanyaan teknis, balas email ini atau hubungi tim recruitment.



---

## Cara Kandidat Menyimpan Hasil Tes

Jangan push hasil pekerjaan ke repository ini.

Sebagai kandidat, Anda wajib:

1. Buka [GitHub](https://github.com) lalu klik **New repository**.
2. Buat repository baru dengan **nama Anda sendiri** (misalnya: `namakandidat-it-app-support-test`).
3. Atur repository menjadi **Public**.
4. Centang opsi **Add README file** agar ada petunjuk awal.
5. Klik **Create repository**.
6. Push seluruh hasil pekerjaan (Node.js project, SQL, README.md Anda sendiri) ke repo tersebut.
7. Kirimkan **link repository GitHub publik Anda** kepada tim recruitment melalui email.

Dengan demikian, setiap kandidat akan memiliki repo jawaban masing-masing.
