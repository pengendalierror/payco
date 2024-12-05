# PAYCO Register Bot

Bot otomatis untuk registrasi akun PAYCO menggunakan email temporary dari Kuku.lu.

## Persyaratan

- Python 3.10.x
- Windows OS
- Koneksi internet yang stabil

## Instalasi

1. Extract semua file ke folder yang diinginkan
2. Double click file `install.bat` untuk:
   - Membuat virtual environment
   - Menginstall semua dependencies yang diperlukan
   - Menginstall browser Chromium
   - Membuat file `.env` dari template
3. Edit file `.env` dan isi dengan kredensial yang diperlukan:

## ENV

1. DOMAIN

   * Kosongkan jika ingin menggunakan domain random
   * Isi domain jika ingin menggunakan domain email yg spesifik
2. PASSWORD

   * Password yg akan digunakan untuk pembuatan akun Payco

## InstAddr Kredensial

Untuk mendapatkan kredensial InstAddr:

1. Buka website [InstAddr](https://m.kuku.lu/)
2. Login ke akun anda
3. Buka Developer Tools (F12)
4. Pergi ke tab Network
5. Isi kolom filter dengan **recv._aj**
6. Klik inbox/Kotak masuk
7. Akan muncul url di DevTools
8. Klik URL yg ada teks **recv._ajax**
9. Klik Payload, nanti akan muncul data yg dibutuhkan.
10. Untuk mendapatkan SESSION_HASH, di menu DevTools Pergi ke tab Application > Cookies

## 🚀 Cara Penggunaan

1. Double click file `start.bat` untuk menjalankan bot
2. Kirimkan Hardware ID ke developer untuk mendapatkan lisensi
3. Letakkan file lisensi (`.license`) di folder yang sama dengan script
4. Jalankan kembali `start.bat`
5. Masukkan jumlah akun yang ingin dibuat
6. Bot akan mulai membuat akun secara otomatis

## 📁 Output

- Akun yang berhasil dibuat akan disimpan di folder `accounts`
- Format file: `accounts_YYYY-MM-DD.txt`
- Format isi file: `email:password`

## ⚠️ Catatan Penting

- Pastikan kredensial Kuku.lu selalu up-to-date
- Jangan menutup browser saat bot sedang berjalan
- Gunakan VPN jika diperlukan untuk menghindari rate limit
- Backup file `.env` dan `.license` sebelum reinstall


## 🆘 Troubleshooting

### Bot tidak bisa membuat email

- Periksa kredensial Kuku.lu di file `.env`
- Pastikan session Kuku.lu masih aktif
- Coba gunakan VPN jika terkena rate limit

### Lisensi Invalid

- Pastikan file `.license` ada di folder yang benar
- Pastikan menggunakan file lisensi yang sesuai dengan Hardware ID
- Hubungi developer untuk pembaruan lisensi

### Error saat Instalasi

- Pastikan Python 3.10+ terinstall dan ada di PATH
- Jalankan Command Prompt sebagai Administrator
- Hapus folder `venv` dan jalankan ulang `install.bat`
