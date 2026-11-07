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

### Daftar Isi

1. [Materi 1 – Prompt Engineering](#materi-1--prompt-engineering)
2. [Materi 2 – Git dan GitHub](#materi-2--git-dan-github)
3. [Materi 3 – Setup Environment](#materi-3--setup-environment)
4. [Materi 4 – Praktik: Student Task Planner](#materi-4--praktik-student-task-planner)
5. [Poin Penting & Pengetahuan Baru](#-poin-penting--pengetahuan-baru)
6. [Struktur Repository](#-struktur-repository)

---

### Materi 1 – Prompt Engineering

#### Apa itu prompt?

**Prompt** adalah instruksi atau masukan yang diberikan kepada model AI untuk mendapatkan hasil tertentu. Bentuknya beragam: pertanyaan sederhana, kata kunci, instruksi yang rumit, hingga potongan kode.

**Prompt engineering** adalah cara merancang instruksi agar AI memberikan jawaban yang **tepat, relevan, dan layak digunakan**.

#### Context is key

Prompt tanpa konteks menghasilkan jawaban yang melebar dan sulit diprediksi.

| Tanpa konteks | Dengan konteks |
|---|---|
| `Create student task planner` | Prompt yang menjelaskan tujuan, kebutuhan, batasan, dan format hasil yang diinginkan |

#### Struktur prompt yang baik

| Komponen | Fungsi | Contoh pada prompt Student Task Planner |
|---|---|---|
| **Role** | Menetapkan peran AI | *"You are helping me build a beginner-friendly student task planner as a simple web application."* |
| **Task** | Menjelaskan tujuan utama | *Goal*: membuat task planner untuk membantu mahasiswa tahun pertama memantau tugas dan tenggat |
| **Context** | Kebutuhan dan batasan | *Requirements* (daftar tugas, tanggal tenggat, status selesai, filter) dan *Constraints* (HTML, CSS, vanilla JavaScript, tanpa library tambahan) |
| **Format** | Bentuk keluaran | *Output*: kode lengkap tiap file, cara menjalankan, dan cara menguji interaksi utama |
