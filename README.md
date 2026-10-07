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
   
   <img width="494" height="378" alt="SS 01 Select Components" src="https://github.com/user-attachments/assets/97c9cc5a-c238-4550-a092-a17c5b6eddd7" />

2. **Choosing Default Editor:** Memilih editor teks default untuk Git (menggunakan Vim)
   <img width="769" height="589" alt="image" src="https://github.com/user-attachments/assets/26c742ed-92d2-4a56-b1a4-78ab70d9e64d" />

3. **Adjusting Initial Branch Name:** Menentukan nama branch utama default untuk repositori baru menjadi `main.
   <img width="797" height="613" alt="image" src="https://github.com/user-attachments/assets/5ba6132a-20a5-4497-89b8-95425a52450c" />

4. **Adjusting PATH Environment:** Mengatur integrasi Git pada Command Prompt dan perangkat lunak pihak ketiga (*Recommended*)
   <img width="798" height="609" alt="image" src="https://github.com/user-attachments/assets/f925ad52-023c-4bff-ba2b-d3167f9118be" />

5. **Choosing SSH Executable:** Memilih *executable* SSH yang akan digunakan oleh Git (menggunakan OpenSSH eksternal).
  <img width="761" height="585" alt="image" src="https://github.com/user-attachments/assets/db620e02-6a6e-4c10-908f-051742664ad9" />

6. **Choosing HTTPS Transport Backend:** Memilih pustaka SSL/TLS untuk koneksi HTTPS (*Windows Secure Channel library*).
   <img width="775" height="593" alt="image" src="https://github.com/user-attachments/assets/b757916b-a50c-453f-b526-a15ac7c6024a" />

7. **Configuring Line Ending Conversions:** Memilih format konversi baris akhir (*Checkout Windows-style, commit Unix-style line endings*).
   <img width="810" height="621" alt="image" src="https://github.com/user-attachments/assets/c2e8e463-055d-4308-a3c5-ae89b1ea159a" />

8. **Configuring Terminal Emulator:** Memilih emulator terminal yang akan digunakan dengan Git Bash (menggunakan MinTTY).
   <img width="820" height="627" alt="image" src="https://github.com/user-attachments/assets/36d45c36-9c7a-4ce4-828b-51de0fe0f05e" />

9. **Choosing Default Behavior of Git Pull:** Memilih perilaku default saat menjalankan perintah `git pull` (*Merge*).
  <img width="806" height="621" alt="image" src="https://github.com/user-attachments/assets/fd18abf1-659f-4f7d-9005-1a781fa53ee5" />

10. **Choosing Credential Helper:** Memilih pengelola kredensial untuk menyimpan otentikasi Git (*Git Credential Manager*).
    <img width="818" height="629" alt="image" src="https://github.com/user-attachments/assets/89d0eaab-a64a-4354-a835-93e5535c712a" />
    
11. **Configuring Extra Options:** Mengaktifkan opsi *file system caching* (`core.fscache`) untuk meningkatkan performa.
   <img width="801" height="616" alt="image" src="https://github.com/user-attachments/assets/10c0d2d5-36c7-4159-95de-dcbdbadff663" />

12. **Installing:** Proses penyalinan dan ekstraksi berkas instalasi Git ke dalam sistem.
   <img width="814" height="617" alt="image" src="https://github.com/user-attachments/assets/bce0f155-c925-47a7-8d06-206e60ebc5b6" />

13. **Completing the Git Setup Wizard:** Proses instalasi Git telah selesai dilakukan.
    <img width="793" height="607" alt="image" src="https://github.com/user-attachments/assets/76ce364f-daa7-4fc6-b66e-6b9e14d9bc62" />

14. **Uji Coba Perintah Git:** Memeriksa daftar perintah utama Git melalui Command Prompt dengan perintah `git`.
    <img width="797" height="607" alt="image" src="https://github.com/user-attachments/assets/3aeac7fc-59c9-46ef-8651-67fe81961a4c" />

15. **Verifikasi Versi Git:** Memeriksa versi Git yang berhasil terpasang menggunakan perintah `git --version`.
    ![SS 15 Version Check](tempel_SS_di_sini) 

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
