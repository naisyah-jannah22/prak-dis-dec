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
1. **License Agreement:** Menyetujui lisensi penggunaan Git.
  <img width="496" height="377" alt="image" src="https://github.com/user-attachments/assets/50d4a021-e54d-424e-b646-657a5bd18f9a" />

2. **Select Destination Location:** Menentukan folder instalasi di `C:\Program Files\Git`.
   ![SS 02 Path](tempel_SS_di_sini)
3. **Select Components:** Memilih komponen utama (Git Bash, Git GUI, dll).
  img width="494" height="378" alt="image" src="https://github.com/user-attachments/assets/97c9cc5a-c238-4550-a092-a17c5b6eddd7" /><

4. **Choosing Default Editor:** Memilih editor teks default untuk Git.
   ![SS 04 Editor](tempel_SS_di_sini)
5. **Adjusting Initial Branch Name:** Menentukan nama branch utama default (`main`).
   ![SS 05 Branch](tempel_SS_di_sini)
6. **Adjusting PATH Environment:** Mengatur integrasi Git pada Command Prompt dan terminal.
   ![SS 06 PATH](tempel_SS_di_sini)
7. **Configuring Line Ending Conversions:** Memilih format konversi baris (`core.autocrlf`).
   ![SS 07 Line Ending](tempel_SS_di_sini)
8. **Configuring Extra Options:** Mengaktifkan opsi *file system caching*.
   ![SS 08 Extra Options](tempel_SS_di_sini)
9. **Verifikasi Instalasi:** Memeriksa versi Git melalui terminal.
   * Perintah: `git --version`
   ![SS 09 Version Check](tempel_SS_di_sini)

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
