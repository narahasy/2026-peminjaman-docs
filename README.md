# 2026-peminjaman-docs

Dokumentasi lengkap untuk Proyek Sistem Peminjaman (Fullstack).

## 1. Analisis Masalah (Studi Kasus)
Sistem ini dibuat untuk mendigitalisasi proses peminjaman agar lebih terstruktur. Fokus utama adalah pengelolaan data pelanggan (Customer) yang mencakup:
- Pencatatan biodata lengkap (Nama, Email, Alamat, No. Telp).
- Status keanggotaan (Active/Inactive).
- Riwayat pendaftaran pelanggan.

## 2. Arsitektur Sistem
Proyek ini menggunakan arsitektur **Client-Server**:
- **Backend:** ASP.NET Core 8 (REST API) dengan Database SQLite.
- **Frontend:** React.js (Web Interface).
- **Mobile:** Flutter (Development).
- **Database:** Entity Framework Core (Code First Approach).

## 3. Spesifikasi API (API Spec)
Berikut adalah endpoint utama yang dikembangkan di modul Backend:

| Method | Endpoint | Deskripsi |
|-------------------------------|
| GET | `/api/Customers` | Mengambil semua data customer |
| GET | `/api/Customers/{id}` | Mengambil detail satu customer |
| POST | `/api/Customers` | Menambah customer baru |
| PUT | `/api/Customers/{id}` | Update data customer |
| DELETE | `/api/Customers/{id}` | Menghapus data customer |

## 4. Struktur Data (Entity)
Entitas **Customer** memiliki atribut:
- `Id` (Integer, Primary Key)
- `Name` (String)
- `Email` (String)
- `Phone` (String)
- `Address` (String)
- `Status` (Boolean)
- `CreatedAt` (DateTime)