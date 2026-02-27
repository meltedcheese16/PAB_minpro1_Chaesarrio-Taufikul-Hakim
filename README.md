# ☕ Katalog Kopi @Wakeup.social

Aplikasi Flutter sederhana untuk mengelola katalog kopi dengan fitur CRUD (Create, Read, Delete).

## 📱 Deskripsi Aplikasi

Katalog Kopi @Wakeup.social adalah aplikasi mobile yang dibuat menggunakan Flutter dan Dart. Aplikasi ini memungkinkan pengguna untuk menambahkan, melihat, dan menghapus data kopi. Data disimpan secara lokal menggunakan List (tidak menggunakan database eksternal), sehingga data akan hilang ketika aplikasi ditutup. Cocok untuk pembelajaran dasar Flutter dan state management dengan StatefulWidget.

## ✨ Fitur Aplikasi

| Fitur | Deskripsi |
|-------|-----------|
| **Create (Tambah Kopi)** | Menambahkan data kopi baru melalui form dialog dengan 3 input: Nama Kopi, Jenis Kopi, dan Harga |
| **Read (Lihat Kopi)** | Menampilkan daftar kopi dalam ListView dengan tampilan Card yang menarik |
| **Detail View** | Menampilkan detail kopi ketika card diklik (icon besar, badge jenis, harga) |
| **Delete (Hapus Kopi)** | Menghapus data kopi dengan konfirmasi dialog |
| **Validasi Input** | Semua field wajib diisi sebelum menyimpan |
| **Tema Kopi** | UI dengan warna coklat/cream yang konsisten |
| **Notifikasi** | Snackbar muncul saat berhasil menambah data |

## 🛠️ Widget yang Digunakan

### Layout & Struktur
- `MaterialApp` - Root aplikasi dengan tema
- `Scaffold` - Struktur dasar halaman (AppBar, Body, FAB)
- `StatefulWidget` - Widget dengan state yang bisa berubah

### Input & Form
- `TextField` - Input teks untuk nama, jenis, dan harga kopi
- `TextEditingController` - Mengontrol dan membaca nilai input
- `AlertDialog` - Dialog popup untuk form input dan konfirmasi

### Tampilan Data
- `ListView.builder` - Menampilkan list data secara efisien
- `Card` - Container untuk setiap item kopi dengan elevation
- `ListTile` - Layout item dengan leading, title, subtitle, trailing
- `InkWell` - Membuat card bisa diklik dengan efek ripple
- `Dialog` - Menampilkan detail view kopi

### UI Components
- `AppBar` - Header aplikasi dengan judul dan gradient
- `FloatingActionButton` - Tombol tambah kopi di pojok kanan bawah
- `Icon` & `IconButton` - Icon kopi, delete, dan indikator
- `Container` - Container dengan decoration (warna, border radius, shadow)
- `BoxDecoration` - Gradient, rounded corners, shadow
- `SnackBar` - Notifikasi singkat di bawah layar

### Theme & Styling
- `LinearGradient` - Gradient warna pada AppBar dan Card
- `BorderRadius` - Sudut melengkung pada Card dan Button
- `Color` - Custom color palette (coffeeDark, coffeeMedium, coffeeLight, coffeeCream)

## 🚀 Cara Menjalankan

1. Pastikan Flutter sudah terinstall
2. Clone repository ini
3. Jalankan perintah:
   ```bash
   flutter pub get
   flutter run
