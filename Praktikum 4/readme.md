#  Praktikum 2: Autentikasi (Laravel Breeze)

##  Identitas Mahasiswa
**Nama:** Andika Haikal Syahputra  
**NIM:** 4523210016  
**Dosen Pengampu:** Adi Wahyu Pribadi, S.Si., M.Kom  

---

##  Bagian 1: Konsep & Filosofi Autentikasi

### 🔹 a. Filosofi Autentikasi — *“Siapa Anda?”*
Autentikasi adalah proses untuk memverifikasi identitas pengguna.  
Metode yang umum digunakan:
- **Sesuatu yang diketahui:** Password.  
- **Sesuatu yang dimiliki:** Ponsel (OTP).  
- **Sesuatu yang melekat:** Sidik jari.

> **Autentikasi ≠ Otorisasi**
> - Autentikasi → Menentukan siapa pengguna.
> - Otorisasi → Menentukan apa yang boleh dilakukan pengguna.

**Analogi:**
- Autentikasi: Menunjukkan kartu mahasiswa ke satpam kampus.  
- Otorisasi: Hanya bisa masuk ke gedung fakultas sendiri.

---

### 🔹 b. Alur Kerja Login
1. Pengguna mengetik email dan password.  
2. Sistem mencari pengguna di database.  
3. Password diverifikasi melalui hashing.  
4. Jika cocok → login berhasil.  
5. Session dan Cookie digunakan untuk mengingat status login.

---

### 🔹 c. Keamanan Autentikasi
- **Password Hashing:** Laravel menggunakan algoritma kuat seperti *Bcrypt* dan *Argon2* untuk mencegah pembalikan password.  
- **CSRF Protection:** Token `@csrf` digunakan untuk mencegah serangan *Cross-Site Request Forgery.*

---

### 🔹 d. Cookies & Sessions
**Analogi:** Setelah login, pengguna mendapat “stempel konser” (Cookie).  
Saat berpindah halaman, Laravel mengenali pengguna melalui session ID di Cookie.

---

### 🔹 e. Diagram Sederhana


#  Foto Dokumentasi Praktikum 2: Autentikasi (Laravel Breeze)





<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/48542434-975f-472e-886a-0bebb5621287" />






<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9a24fdb0-f1b5-40e1-aa88-c1876a1f5368" />
