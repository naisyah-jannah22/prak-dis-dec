# Laporan Praktikum Sistem Terdistribusi dan Terdesentralisasi
## Minggu 01: Pengenalan Sistem Terdistribusi dan Terdesentralisasi - Git dan GitHub

### Identitas Mahasiswa
* **Nama:** Naisyah Izzatul Jannah K.
* **NIM:** 255410040
* **Kelas:** Informatika

---

### A. Tujuan
1. Memahami konsep dasar Version Control System (VCS) dan platform kolaborasi GitHub.
2. Menguasai alur instalasi serta konfigurasi opsi-opsi utama Git di sistem operasi Windows.
3. Mampu mengelola repository lokal, repository akun pribadi, repository organisasi, serta melakukan alur kerja kolaborasi (*fork*, *clone*, *branching*, *pull request*).

---

### B. Dasar Teori
* **Git** adalah Distributed Version Control System (DVCS) yang mencatat riwayat perubahan berkas secara lokal maupun terdistribusi.
* **GitHub** adalah platform web penyimpan repository Git yang menyediakan fitur manajemen proyek, kolaborasi tim, organisasi, serta penggabungan kode via *Pull Request*.

---

### C. Langkah Kerja & Bukti Praktikum

#### 1. Instalasi Aplikasi Git (`01-install-git.md`)
Proses instalasi Git for Windows dilakukan melalui wizard setup langkah demi langkah:

1. **Select Components:** Memilih komponen utama untuk diinstal seperti *Windows Explorer integration*, *Git LFS*, dan *Scalar*.
<img width="781" height="579" alt="image" src="https://github.com/user-attachments/assets/1af36142-f912-4f06-b6f8-8766a3641a82" />

2. **Choosing Default Editor:** Memilih editor teks default untuk Git (menggunakan Vim).
<img width="769" height="589" alt="image" src="https://github.com/user-attachments/assets/78a2486d-c530-4e1d-8dab-164b8dd29e0a" />

3. **Adjusting Initial Branch Name:** Menentukan nama branch utama default untuk repositori baru menjadi `main`.
<img width="797" height="613" alt="image" src="https://github.com/user-attachments/assets/8c3a773e-8f2c-419a-b1b9-4d4ce6fa088e" />

4. **Adjusting PATH Environment:** Mengatur integrasi Git pada Command Prompt dan perangkat lunak pihak ketiga (*Recommended*).
<img width="798" height="609" alt="image" src="https://github.com/user-attachments/assets/76e1c3e9-5b1c-4b36-84f4-0ccda4437894" />

5. **Choosing SSH Executable:** Memilih *executable* SSH yang akan digunakan oleh Git (menggunakan OpenSSH eksternal).
<img width="761" height="585" alt="image" src="https://github.com/user-attachments/assets/518a52aa-2dad-407e-92e1-e776fb71ad6d" />

6. **Choosing HTTPS Transport Backend:** Memilih pustaka SSL/TLS untuk koneksi HTTPS (*Windows Secure Channel library*).
<img width="775" height="593" alt="image" src="https://github.com/user-attachments/assets/0fad8183-3fa2-4d45-b4c8-92ac213250a1" />

7. **Configuring Line Ending Conversions:** Memilih format konversi baris akhir (*Checkout Windows-style, commit Unix-style line endings*).
<img width="810" height="621" alt="image" src="https://github.com/user-attachments/assets/1399c1be-7d5d-4000-a804-a5d1c764e378" />

8. **Configuring Terminal Emulator:** Memilih emulator terminal yang akan digunakan dengan Git Bash (menggunakan MinTTY).
<img width="820" height="627" alt="image" src="https://github.com/user-attachments/assets/c8d660a6-905e-41b4-9e3d-389e30f0598a" />

9. **Choosing Default Behavior of Git Pull:** Memilih perilaku default saat menjalankan perintah `git pull` (*Merge*).
<img width="806" height="621" alt="image" src="https://github.com/user-attachments/assets/8604dab3-b333-4e5c-9139-50c55d5596c4" />

10. **Choosing Credential Helper:** Memilih pengelola kredensial default untuk menyimpan otentikasi Git (*Git Credential Manager*).
<img width="818" height="629" alt="image" src="https://github.com/user-attachments/assets/07465599-c67d-40ff-a4e6-3d904a95adf7" />

11. **Configuring Extra Options:** Mengaktifkan opsi *file system caching* (`core.fscache`) untuk meningkatkan performa.
<img width="801" height="616" alt="image" src="https://github.com/user-attachments/assets/f3cd30fb-cea5-41f1-971e-da7a269a6c2e" />

12. **Installing:** Proses penyalinan dan ekstraksi berkas instalasi Git ke dalam sistem.
<img width="814" height="617" alt="image" src="https://github.com/user-attachments/assets/42b83239-fcac-4ca4-9f93-4549e17b4f57" />

13. **Completing the Git Setup Wizard:** Proses instalasi Git telah selesai dilakukan.
<img width="793" height="607" alt="image" src="https://github.com/user-attachments/assets/386848c2-df5a-4959-a636-31106b83d847" />

14. **Uji Coba Perintah Git:** Memeriksa daftar perintah utama Git melalui Command Prompt dengan perintah `git`.
 <img width="797" height="607" alt="image" src="https://github.com/user-attachments/assets/27f5371d-8b3d-4e09-85d8-1ebe805e8a22" />

15. **Verifikasi Versi Git:** Memeriksa versi Git yang berhasil terpasang menggunakan perintah `git --version`.
 <img width="940" height="634" alt="image" src="https://github.com/user-attachments/assets/c3b94ffd-444b-4276-ab7e-66ea3046f253" />

<img width="940" height="117" alt="image" src="https://github.com/user-attachments/assets/0e9d2232-f9eb-42ef-8a05-f011c16a24eb" />

---
#### 2. Konfigurasi Git (`02-konfigurasi-git.md`)
Melakukan pengaturan identitas global pengguna pada terminal/Git Bash:
1. **Konfigurasi Nama Pengguna:**
   * Perintah: `git config --global user.name "Naisyah Izzatul Jannah K."`
  <img width="655" height="115" alt="image" src="https://github.com/user-attachments/assets/7778f080-4bc2-4cb4-974f-f9a14b1d6862" />

2. **Konfigurasi Alamat Email:**
   * Perintah: `git config --global user.email "naisyahjannah@gmail.com"`
  <img width="650" height="137" alt="image" src="https://github.com/user-attachments/assets/9cf22a70-a28a-43c1-ae11-4641b4e6a226" />

3. **Pengecekan Daftar Konfigurasi:**
   * Perintah: `git config --list`
 <img width="649" height="427" alt="image" src="https://github.com/user-attachments/assets/30683519-004a-4dea-9b0f-a8cd25f4df71" />

---

#### 3. Mengelola Repository Sendiri - Akun Pribadi (`03-mengelola-repo-sendiri-account.md`)
Melakukan pendaftaran akun dan latihan perintah dasar Git pada repository lokal:
1. **Pendaftaran Akun GitHub:**
   Pengisian form pendaftaran akun baru pada situs GitHub dengan username `naisyah-jannah22`. Terjadi kendala aturan penulisan username yang kemudian berhasil diselesaikan hingga valid.
   <img width="958" height="538" alt="image" src="https://github.com/user-attachments/assets/67b27443-cac6-4cd0-9545-c7c23c3edc5d" />

2. **Inisialisasi Repository Lokal:**
   * Perintah: `git init`
   <img width="504" height="241" alt="image" src="https://github.com/user-attachments/assets/de007b55-7a7e-4051-8b3a-db79bbca1336" />

3. **Memeriksa Status Pelacakan:**
   * Perintah: `git status`
  <img width="546" height="259" alt="image" src="https://github.com/user-attachments/assets/93fdd9a5-c95f-4d5c-875f-a84203d8dac6" />

4. **Menambahkan File ke Staging Area:**
   * Perintah: `git add .`
   <img width="346" height="186" alt="image" src="https://github.com/user-attachments/assets/b3f6357b-042a-441d-8b96-6b4c5c033f3e" />

5. **Menyimpan Perubahan (Commit):**
   * Perintah: `git commit -m "Membuat laporan minggu 01"`
  <img width="724" height="206" alt="image" src="https://github.com/user-attachments/assets/8879925b-e661-429b-9a98-c925f055fb2d" />

6. **Melihat Riwayat Commit:**
   * Perintah: `git log --oneline`
   <img width="682" height="241" alt="image" src="https://github.com/user-attachments/assets/119e0737-51b0-4cb4-8bc5-8adda0491d35" />

---

#### 4. Mengelola Repository Sendiri - Organisasi (`03-mengelola-repo-sendiri-organisasi.md`)
Membuat dan mengelola repository di bawah naungan Organisasi GitHub:
1. **Membuat/Masuk ke Organisasi GitHub:**
   Membuat atau bergabung dengan akun organisasi di GitHub.
   ![SS Akun Organisasi](tempel_SS_di_sini)
2. **Membuat Repository Organisasi:**
   Membuat repository baru milik organisasi.
   ![SS Repo Organisasi](tempel_SS_di_sini)
3. **Manajemen Akses & Anggota Organisasi:**
   Mengatur peran (*role*) dan hak akses anggota tim di dalam organisasi.
   ![SS Anggota Organisasi](tempel_SS_di_sini)

---

#### 5. Kolaborasi & Workflow GitHub (`04-kolaborasi.md`)
Melakukan simulasi dan praktik alur kerja kolaborasi proyek open-source/tim di GitHub:
1. **Fork Repository:**
   Membuat duplikasi (*fork*) dari repository pengguna lain/utama ke akun pribadi.
   ![SS Fork Repository](tempel_SS_di_sini)
2. **Clone Repository Lokal:**
   Mendownload repository hasil fork ke komputer lokal.
   * Perintah: `git clone <URL_Repository>`
   ![SS Git Clone](tempel_SS_di_sini)
3. **Membuat Branch Baru:**
   Membuat dan berpindah ke cabang fitur (*feature branch*) baru untuk pengerjaan tugas.
   * Perintah: `git checkout -b fitur-baru`
   ![SS Git Branch](tempel_SS_di_sini)
4. **Push Changes ke Remote Branch:**
   Mengunggah perubahan dari branch lokal ke GitHub.
   * Perintah: `git push origin fitur-baru`
   ![SS Git Push Branch](tempel_SS_di_sini)
5. **Membuat & Menggabungkan Pull Request (PR):**
   Mengajukan *Pull Request* pada halaman GitHub dan melakukan proses *Merge* perubahan ke branch utama.
   ![SS Pull Request dan Merge](tempel_SS_di_sini)

---

### D. Hasil Praktikum & Link Pengumpulan
* **URL Repository Utama:** `https://github.com/naisyah-jannah22/prak-dis-dec`
* **URL Laporan Minggu 1:** `https://github.com/naisyah-jannah22/prak-dis-dec/tree/main/01`

---

### E. Kesimpulan
Praktikum minggu ke-1 telah berhasil menyelesaikan seluruh alur kerja Git dan GitHub, mulai dari instalasi bertahap, konfigurasi identitas pengguna, pengelolaan repository lokal pada akun pribadi maupun organisasi, hingga alur kerja kolaborasi terdistribusi (*fork*, *clone*, *branching*, dan *pull request*).
