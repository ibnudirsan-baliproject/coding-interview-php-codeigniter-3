# Deskripsi
Buatlah sebuah API tanpa autentikasi menggunakan CodeIgniter 3 yang menggunakan model Employee dengan tabel `employees`. API ini harus menyediakan fitur CRUD dasar untuk mengelola data karyawan.

## Struktur Tabel Employee
Tabel `employees` memiliki kolom sebagai berikut:

- `id` (integer, primary key, auto-increment)
- `fullname` (string, required)
- `email` (string, unique, required)
- `mobilephone` (string, required)
- `date_of_birth` (date, required)
- `address` (text, required)

## Endpoint Employee
### [GET] `/api/employee`
Mendapatkan daftar semua karyawan.
#### Response JSON:
```json
{
    "status": "success",
    "data": [
        {
            "id": 1,
            "fullname": "John Doe",
            "email": "john@example.com",
            "mobilephone": "08123456789",
            "date_of_birth": "1990-01-01",
            "address": "Jl. Contoh No.1"
        }
    ]
}
