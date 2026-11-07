> Dokumentasi workshop **"From AI to GitHub: Building with AI, Managing Change with GitHub"**

---

## 👤 Identitas Peserta

| | |
|---|---|
| **Nama Lengkap** | [Muhammad Rayan] |
| **Kelompok** | [Dreadout] |
| **Hari / Tanggal** | Day 1 – [7 November 2026] |

---

## 📖 Deskripsi Repository

Repository ini berisi dokumentasi kegiatan workshop **Building with AI, Managing Change with GitHub** yang disampaikan oleh **Nugi Farhan (Senior Product Designer)**. Di dalamnya terdapat materi yang disampaikan, rangkuman catatan, serta poin-poin penting yang dipelajari selama workshop, mulai dari *prompt engineering* hingga penggunaan Git dan GitHub untuk mengelola perubahan kode.

## 🎯 Tujuan Repository

- Mendokumentasikan seluruh materi dan catatan workshop secara rapi dan terstruktur dalam satu tempat.
- Menjadi bahan referensi belajar untuk mengulang kembali materi prompt engineering, Git, dan GitHub.
- Menjadi latihan langsung membuat repository, menulis dokumentasi, dan mengunggahnya ke GitHub sesuai ketentuan tugas.

## 🗓️ Tentang Kegiatan Workshop

| | |
|---|---|
| **Judul** | From AI to GitHub – Building with AI, Managing Change with GitHub |
| **Pemateri** | Nugi Farhan, Senior Product Designer |
| **Topik 1** | Membuat dan mengembangkan sesuatu dengan bantuan AI (*prompt engineering*) |
| **Topik 2** | Manajemen perubahan dan kolaborasi dengan Git & GitHub |
| **Proyek latihan** | Student Task Planner (aplikasi web sederhana) |

### Capaian Pembelajaran

Setelah workshop, peserta diharapkan dapat:

1. Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
2. Membedakan apa itu Git dan GitHub.
3. Mengidentifikasi *repository*, *commit*, *branch*, dan *pull request*.
4. Melakukan *version controlling*.

---

## 📚 Dokumentasi Workshop
### Materi 1 – Prompt Engineering

#### Apa itu prompt?

**Prompt** adalah instruksi atau masukan yang diberikan kepada model AI untuk mendapatkan hasil tertentu. Bentuknya beragam: pertanyaan sederhana, kata kunci, instruksi yang rumit, hingga potongan kode.

**Prompt engineering** adalah cara merancang instruksi agar AI memberikan jawaban yang **tepat, relevan, dan layak digunakan**.

#### Context is key

Prompt tanpa konteks menghasilkan jawaban yang melebar dan sulit diprediksi.

| Tanpa konteks | Dengan konteks |
|---|---|
| `Create student task planner` | Prompt yang menjelaskan tujuan, kebutuhan, batasan, dan format hasil yang diinginkan |

### Materi 2 – Git dan GitHub

#### Apa itu Git?

**Git** adalah *version control system* yang melacak **siapa**, **kapan**, dan **apa saja** yang diubah dalam suatu file. Git diciptakan oleh **Linus Torvalds** pada tahun 2005 untuk mencatat setiap perubahan yang terjadi pada file.

### Materi 3 – Setup Environment

#### Setup Git

1. Install Git (cari di Google: "install git").
2. Pilih versi yang sesuai dengan perangkat.
3. Buka terminal / cmd, lalu cek versi:
   ```bash
   git --version
   # git version 2.xx.xx
   ```
4. Atur identitas Git:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```
5. Cek konfigurasi:
   ```bash
   git config --global --list
   ```

#### Setup VS Code

1. Install VS Code.
2. Buka VS Code.
3. Tekan `Command+Shift+P` / `Ctrl+Shift+P`.
4. Cari **Shell Command: Install 'code' command in PATH**.
5. Buka terminal dan jalankan `code --version`.

#### Membuat SSH Key

```bash
ssh-keygen -t ed25519 -C "email@domain.com"
```

- Saat diminta lokasi file, tekan **Enter** untuk menerima lokasi default (`~/.ssh/id_ed25519`).
- Saat diminta passphrase, masukkan passphrase yang aman (atau tekan Enter dua kali untuk tanpa passphrase).

> **Ed25519** adalah skema tanda tangan kurva eliptik (EdDSA pada kurva Curve25519, dibuat oleh Daniel J. Bernstein pada 2011) yang dirancang untuk keamanan dan performa tinggi serta tahan terhadap serangan implementasi kriptografi yang umum.

### Materi 4 – Praktik: Student Task Planner

Proyek latihan: **Student Task Planner**, aplikasi web sederhana untuk membantu mahasiswa memantau tugas dan tenggat waktu.

Alur kerja yang dipraktikkan:

1. Install platform AI (Claude, Antigravity, ChatGPT).
2. Tulis prompt untuk membuat web / aplikasi.
3. Tambahkan proyek ke Git dengan `git init`.
4. *Commit* dan *push* ke GitHub.
5. Lakukan perubahan pada proyek.
6. *Commit* dan *push* kembali ke GitHub.

```bash
git init
git add .
git commit -m "Initial commit: student task planner"
git remote add origin git@github.com:<username>/<nama-repository>.git
git push origin main

# setelah melakukan perubahan
git add .
git commit -m "Deskripsi perubahan"
git push origin main
```

---

## 💡 Poin Penting & Pengetahuan Baru

**Tentang prompt engineering**

- Prompt yang spesifik dan berkonteks menghasilkan jawaban AI yang lebih relevan dibanding instruksi singkat.
- Struktur **Role → Task → Context → Format** membantu menyusun prompt yang jelas.
- Menambahkan batasan (*constraints*) dan format keluaran membuat hasil AI lebih mudah diprediksi dan dikontrol.
- Hasil AI tetap perlu diverifikasi, seperti yang ditegaskan di akhir contoh prompt: jangan mengklaim aplikasi berjalan sebelum perilakunya diuji.

**Tentang Git dan GitHub**

- **Git** bekerja secara lokal untuk melacak perubahan, sedangkan **GitHub** adalah tempat menyimpan repository secara online dan berkolaborasi.
- Perubahan melewati tiga area: *working directory* → *staging area* → *repository (.git)*.
- Alur dasar yang paling sering dipakai: `git add` → `git commit` → `git push`.
- Setiap commit mencatat siapa, kapan, dan apa yang berubah, sehingga riwayat proyek bisa dilacak dan dipulihkan.
- SSH key memungkinkan autentikasi ke GitHub tanpa memasukkan kredensial berulang kali.

**Istilah penting**

| Istilah | Arti singkat |
|---|---|
| **Repository** | Tempat penyimpanan proyek beserta seluruh riwayat perubahannya |
| **Commit** | Catatan (snapshot) perubahan yang disimpan ke repository, disertai pesan |
| **Branch** | Cabang pengembangan terpisah agar perubahan bisa dikerjakan tanpa mengganggu versi utama |
| **Pull Request** | Permintaan untuk menggabungkan perubahan dari satu branch ke branch lain, biasanya ditinjau dulu oleh tim |

---

## 🗂️ Struktur Repository

```text
Day-1-(Nama_Kelompok)_Nama Lengkap/
├── README.md        # Dokumentasi utama workshop (file ini)
└── ...              # Tambahkan file lain (mis. proyek Student Task Planner, tangkapan layar) di sini
```

---
