# prak-dis-dec.
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
   ![SS 01 License](tempel_SS_di_sini)
2. **Select Destination Location:** Menentukan folder instalasi di `C:\Program Files\Git`.
   ![SS 02 Path](tempel_SS_di_sini)
3. **Select Components:** Memilih komponen utama (Git Bash, Git GUI, dll).
   ![SS 03 Components](tempel_SS_di_sini)
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
   ![SS Config Name](tempel_SS_di_sini)
2. **Konfigurasi Alamat Email:**
   * Perintah: `git config --global user.email "email_kamu@gmail.com"`
   ![SS Config Email](tempel_SS_di_sini)
3. **Pengecekan Daftar Konfigurasi:**
   * Perintah: `git config --list`
   ![SS Config List](tempel_SS_di_sini)

---

#### 3. Mengelola Repository Sendiri - Akun Pribadi (`03-mengelola-repo-sendiri-account.md`)
Melakukan latihan perintah dasar Git pada repository lokal dan akun pribadi:
1. **Inisialisasi Repository Lokal:**
   * Perintah: `git init`
   ![SS Git Init](tempel_SS_di_sini)
2. **Memeriksa Status Pelacakan:**
   * Perintah: `git status`
   ![SS Git Status](tempel_SS_di_sini)
3. **Menambahkan File ke Staging Area:**
   * Perintah: `git add .`
   ![SS Git Add](tempel_SS_di_sini)
4. **Menyimpan Perubahan (Commit):**
   * Perintah: `git commit -m "Membuat laporan minggu 01"`
   ![SS Git Commit](tempel_SS_di_sini)
5. **Melihat Riwayat Commit:**
   * Perintah: `git log --oneline`
   ![SS Git Log](tempel_SS_di_sini)

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
* **URL Repository Utama:** `https://github.com/naisyahizzatul25-tech/prak-dis-dec`
* **URL Laporan Minggu 1:** `https://github.com/naisyahizzatul25-tech/prak-dis-dec/tree/main/01`

---

### E. Kesimpulan
Praktikum minggu ke-1 telah berhasil menyelesaikan seluruh alur kerja Git dan GitHub, mulai dari instalasi bertahap, konfigurasi identitas pengguna, pengelolaan repository lokal pada akun pribadi maupun organisasi, hingga alur kerja kolaborasi terdistribusi (*fork*, *clone*, *branching*, dan *pull request*).
