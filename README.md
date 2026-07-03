# Automatic Response and Confirm Registration Google Form



Otomasi Respon dan Konfirmasi via email untuk pendaftaran menggunakan Google Form dengan dukungan multi-platform (Google Apps Script) untuk otomasi respon dan konfirmasinya.

## 📋 Daftar Isi

* [Arsitektur Sistem](#-arsitektur-sistem)
* [Persyaratan Sistem](#-persyaratan-sistem)
* [Instalasi](#-instalasi)
* [Penggunaan](#-penggunaan)
* [Database Schema](#-database-schema)
* [Keamanan](#-keamanan)
* [Pengembangan](#-pengembangan)
* [Troubleshooting](#-troubleshooting)
* [Lisensi](#-lisensi)

## 🏗️ Arsitektur Sistem

### **Versi Google Apps Script (auto-regist/)**

* **Frontend**: Google Form
* **Backend**: Google Apps Script (GAS)
* **Database**: Google Sheets API
* **Storage**: Google Drive
* **Authentication**: Google OAuth

## 💻 Persyaratan Sistem

### **Google Apps Script**

* Google Account dengan Apps Script enabled
* Google Sheets untuk database
* Google Drive untuk file storage
* Modern web browser

## 📦 Instalasi

### **1. Google Apps Script Version**

\# Buat Google Form dan Google Sheet, Google Apps Script project baru

\# 1. Buka https://docs.google.com/forms
# 2. Klik/Pilih Blank Form
# 3. Buat form registrasi

\# 4. Berikan nama form, deskripsi dan pertanyaan-pertanyaannya

\# 5. Pastikan pertanyaan mana yang harus diisi, mana yang opsional

\# 6. Setelah selesai, publish form tersebut

\# 7. Pastikan form tersebut dapat diakses oleh siapa saja (everyone)

\# 8. Lakukan tes pengisian data, sebelum di rilis

\# 9. Cek hasil pengisian data pada tab Response

\#10. Hubungkan data tersebut ke google sheet, link to sheets

\#11. Create a new spreadsheet, untuk membuat google sheet baru (awal)

\#12. Dari google sheet tsb. masukkan script dari menu Extensions -> Apps Script
#13. Beri nama script-nya, copy isi Code.gs ke editor
#14. Ganti alamat email admin dengan email admin Anda
#15. Sesuaikan juga kolom di sheet yang akan diambil datanya

\#16. Agar script ini dapat dijalankan otomatis, lakukan lewat trigger

\#17. Pilih menu Triggers, tambahkan trigger

\#18. Pada event type, pilih 'on form submit' kemudian simpan trigger tsb

\#19. Klik Advanced pada jendela permohonan akses, pilih 'Go to project' dan klik Continue

\#20. Otorisasi selesai

\#21. Kembali ke form registrasi, lakukan pengisian data selanjutnya untuk mengetes jalannya script

\#22. Perbaiki script bila ada kesalahan. Selesai.

```



## 🎮 Penggunaan

\# Jalankan google form, setelah di-submit maka akan otomatis terkirim respon dan konfirmasi email dari admin

```



## 🗄️ Database Schema

### **Google Sheets Structure**

**# Sesuai urutan dalam google form**

```



## 🔒 Keamanan

### **Authentication**

```

\# Google OAuth integration

```



## 🛠️ Pengembangan

### **Project Structure**

```
auto-regist/        # Google Apps Script version
├── Code.gs         # Backend logic
└── README.md
```



### **Testing**

```
# Manual Testing
# Use browser dev tools
```



## 🔧 Troubleshooting

### **Common Issues**

* "Quota exceeded": Check Google Apps Script quotas
* "CORS error": Configure OAuth scopes properly

### **Debug Mode**

```javascript
// Enable debug in browser console
localStorage.setItem('debug', 'true');
```

### **Logs**

* **GAS**: View in Apps Script editor → Executions
* **Browser**: Use developer tools console

```



## 📄 Lisensi

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**u.c.m.e | a simple wrok**

* Contact: yoe.c.me.us@gmail.com

## 🙏 Acknowledgments

* Google Apps Script Team

\---

**Versi**: 1.0.0
**Terakhir Update**: Juni 2026
**Dokumentasi**: README.md

