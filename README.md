# LaraPress - Aplikasi Blog Sederhana

NAMA : Ahmad Farid Akbar

NPM:4523210006

LaraPress adalah aplikasi blog sederhana yang dibangun menggunakan Laravel 12 untuk tujuan pembelajaran dan pengembangan keterampilan web development.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7fc8502f-60ba-4fd3-b716-30a4dd9f7dcc" />

*Tampilan halaman utama LaraPress*

## 📋 Tentang Proyek

Proyek ini dibuat sebagai bagian dari pembelajaran Laravel framework. LaraPress mendemonstrasikan konsep-konsep dasar Laravel seperti routing, views, dan struktur MVC.

## 🚀 Fitur yang Sudah Diimplementasikan

### 1. **Halaman Utama (Welcome Page)**
   - Mengubah tampilan default Laravel menjadi halaman sederhana
   - Menampilkan judul "Selamat Datang di LaraPress"
   - Struktur HTML yang bersih dan minimal

### 2. **Halaman Tentang Kami**
   - Route: `/tentang-kami`
   - Menampilkan informasi tentang LaraPress
   - Menjelaskan tujuan proyek sebagai pembelajaran Laravel 12

### 3. *Kontak*
    -Buat satu halaman statis baru bernama "Kontak".
    -Halaman ini harus bisa diakses melalui URL /kontak.
    -Isi halaman tersebut dengan informasi kontak fiktif (misal: email dan nomor telepon).
    -Jangan lupa tambahkan link navigasi ke dan dari halaman "Kontak" di halaman lainnya.


## 📁 Struktur File yang Dimodifikasi

### File yang Dibuat/Dimodifikasi:

1. **`resources/views/welcome.blade.php`**
   - Mengubah tampilan default Laravel yang kompleks menjadi struktur HTML sederhana
   - Menampilkan pesan sambutan untuk pengunjung blog

2. **`resources/views/about.blade.php`** (BARU)
   - File view baru untuk halaman "Tentang Kami"
   - Berisi informasi tentang LaraPress sebagai proyek pembelajaran

3. **`routes/web.php`**
   - Menambahkan route baru `/tentang-kami` yang mengarah ke view `about.blade.php`

## 🛠️ Langkah-langkah Implementasi

### Step 1: Modifikasi Halaman Welcome
Mengubah file `resources/views/welcome.blade.php` dari tampilan default Laravel (266 baris) menjadi HTML sederhana:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Datang di LaraPress</title>
</head>
<body>
    <h1>Selamat Datang di Blog LaraPress</h1>
    <p>Ini adalah halaman utama dari aplikasi blog kita.</p>
</body>
</html>
```

### Step 2: Membuat Route Baru
Menambahkan route baru di `routes/web.php`:

```php
Route::get('/tentang-kami', function () {
    return view('about');
});
```

### Step 3: Membuat View About
Membuat file baru `resources/views/about.blade.php`:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tentang Kami - LaraPress</title>
</head>
<body>
    <h1>Tentang LaraPress</h1>
    <p>LaraPress adalah aplikasi blog sederhana yang dibuat dengan Laravel 12.</p>
    <p>Proyek ini dibuat untuk tujuan pembelajaran dan pengembangan keterampilan.</p>
</body>
</html>
```

## 🌐 Endpoint yang Tersedia

| Route | Method | Deskripsi |
|-------|--------|-----------|
| `/` | GET | Halaman utama LaraPress |
| `/tentang-kami` | GET | Halaman tentang LaraPress |

## 💻 Teknologi yang Digunakan

- **Framework**: Laravel 12
- **PHP Version**: 8.x
- **Database**: SQLite (default)
- **Frontend**: Blade Template Engine, HTML, CSS
- **Build Tool**: Vite

## 📦 Instalasi

1. Clone repository ini:
```bash
git clone https://github.com/Manggo-rill/PBW.git
cd pro1
```

2. Install dependencies:
```bash
composer install
npm install
```

3. Buat file `.env`:
```bash
cp .env.example .env
```

4. Generate application key:
```bash
php artisan key:generate
```

5. Jalankan development server:
```bash
php artisan serve
```

6. Akses aplikasi di browser:
```
http://localhost:8000
```

## 📸 Screenshot

### Halaman Utama
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/526a9fc4-8e4b-407e-91d8-524fb45cd1c0" />


Halaman utama menampilkan sambutan sederhana kepada pengunjung blog LaraPress.

### Tentang LaraPress
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7fc99210-dfe1-40e1-8c87-63b4cda6fb6b" />


### kontak
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/772203f1-fc62-4f91-a979-d1beab7181d1" />



## 🔄 Git History

Semua perubahan telah di-commit dan di-push ke repository dengan pesan commit yang jelas mengenai setiap modifikasi yang dilakukan.

## 📝 Rencana Pengembangan

- [ ] Menambahkan sistem autentikasi
- [ ] Membuat fitur CRUD untuk artikel blog
- [ ] Menambahkan sistem komentar
- [ ] Implementasi kategori dan tag
- [ ] Membuat dashboard admin
- [ ] Menambahkan styling dengan Tailwind CSS
- [ ] Implementasi search functionality

## 👨‍💻 Pengembang

- **Nama**: Ahmad Farid Akbar 
- **Repository**: https://github.com/Manggo-rill/PBW.git
- **Branch**: main

## 📄 Lisensi

Proyek ini menggunakan lisensi MIT - lihat file LICENSE untuk detail lebih lanjut.

---

**Catatan**: Proyek ini dibuat untuk tujuan pembelajaran. Jangan ragu untuk melakukan fork dan modifikasi sesuai kebutuhan Anda!

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
