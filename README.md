# Katalog Kopi @Wakeup.social


<img width="1311" height="887" alt="image" src="https://github.com/user-attachments/assets/fb628e0d-2b96-41bb-964b-71b9340ae174" />

## Deskripsi Aplikasi

Katalog Kopi @Wakeup.social adalah aplikasi mobile yang dibuat menggunakan Flutter dan Dart. Aplikasi ini memungkinkan pengguna untuk menambahkan, melihat, dan menghapus data kopi. Data disimpan secara lokal menggunakan List (tidak menggunakan database eksternal), sehingga data akan hilang ketika aplikasi ditutup. Cocok untuk pembelajaran dasar Flutter dan state management dengan StatefulWidget.

## Fitur Aplikasi

| Fitur | Deskripsi |
|-------|-----------|
| **Create (Tambah Kopi)** | Menambahkan data kopi baru melalui form dialog dengan 3 input: Nama Kopi, Jenis Kopi, dan Harga |
| **Read (Lihat Kopi)** | Menampilkan daftar kopi dalam ListView dengan tampilan Card yang menarik |
| **Detail View** | Menampilkan detail kopi ketika card diklik (icon besar, badge jenis, harga) |
| **Delete (Hapus Kopi)** | Menghapus data kopi dengan konfirmasi dialog |
| **Validasi Input** | Semua field wajib diisi sebelum menyimpan |
| **Tema Kopi** | UI dengan warna coklat/cream yang konsisten |
| **Notifikasi** | Snackbar muncul saat berhasil menambah data |

## Widget yang Digunakan

### Layout & Struktur
- `MaterialApp` - Root aplikasi dengan tema
- `Scaffold` - Struktur dasar halaman (AppBar, Body, FAB)
- `StatefulWidget` - Widget dengan state yang bisa berubah

### Input & Form

<img width="421" height="417" alt="image" src="https://github.com/user-attachments/assets/b382110b-07f5-4572-936e-67f6171d7d6f" />

- `TextField` - Input teks untuk nama, jenis, dan harga kopi
- `TextEditingController` - Mengontrol dan membaca nilai input
- `AlertDialog` - Dialog popup untuk form input dan konfirmasi

### Tampilan Data

<img width="1219" height="495" alt="image" src="https://github.com/user-attachments/assets/5e1722bb-40f6-4daa-abc6-4f16eb5bc661" />

- `ListView.builder` - Menampilkan list data secara efisien
- `Card` - Container untuk setiap item kopi dengan elevation
- `ListTile` - Layout item dengan leading, title, subtitle, trailing
- `InkWell` - Membuat card bisa diklik dengan efek ripple
- `Dialog` - Menampilkan detail view kopi

### **Tombol Delete**

<img width="58" height="56" alt="image" src="https://github.com/user-attachments/assets/2536b1c9-87f7-41e3-8c63-1da18b56c9f0" />


- **Lokasi**: Di sebelah kanan setiap item kopi (trailing di ListTile)
- **Widget**: `IconButton` dengan icon `Icons.delete_outline`
- **Warna**: Merah (`Colors.red`) sebagai indikator aksi berbahaya
- **Style**: Dibungkus dalam `Container` dengan background merah muda (opacity 0.1) dan border radius

<img width="368" height="238" alt="image" src="https://github.com/user-attachments/assets/8dfb970f-9484-4bf9-b2c6-4d79bb103cb9" />
