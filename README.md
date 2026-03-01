# Website Portofolio (HTML + CSS)

Nama   : Dilla Maharani

NIM    : 2409116023

Kelas  : Sistem Informasi A'24

---

## ──★ ˙Deskripsi Website

Website ini merupakan website portofolio statis berbasis HTML + CSS dengan 3 section utama:
- **Home (Hero Section)**: perkenalan singkat + foto
- **About Me**: deskripsi diri, skill (progress bar), dan pengalaman.
- **Certificates**: daftar sertifikat dalam bentuk card.

---

## ──★ ˙Fitur-Fitur
- Navbar (header + menu navigasi ke section)
- Section **Home** (Hero) berisi perkenalan singkat + gambar
- Section **About Me** berisi deskripsi diri, skills dengan progress bar, dan pengalaman 
- Section **Certificates** berisi sertifikat dalam card / grid  
- Menggunakan struktur dasar HTML (html, head, body)  
- Menggunakan CSS untuk styling (warna, background, layout, font, dll)  
- Tampilan rapi dan responsif (dibantu Bootstrap + flex)  
- Website bersifat statis

---

## ──★ ˙Teknologi yang Digunakan
- **HTML5**

  Struktur dasar pembuatan website (html, head, body, section, navbar, dll)
  
- **CSS3**
  
  Styling tampilan (warna, layout, background, font, progress bar, dll)
  
- **Bootstrap 5** (CDN)
  
  Digunakan untuk membantu pembuatan komponen Card pada section Certificates

---

## ──★ ˙Struktur Folder

```
project-folder/
│
├── index.html
├── style.css
└── images/
    ├── mypoto.png
    ├── instagram.png
    ├── inforsa.png
    ├── pengmas.jpg
    └── makrab.png
```

---

## ──★ ˙Tampilan Setiap Section / Fitur

### 1) Navbar
**Fungsi:**
- Menampilkan identitas singkat “My Portofolio ♡”
- Navigasi anchor link ke `#home`, `#about`, `#certificate`
- Menampilkan ikon instagram + username

**Implementasi:**
- Dibuat dengan elemen `header` dan container `.container-navbar`
- Menu menggunakan anchor link:
  - Home 🏡
  - About Me 🙋🏻‍♀️
  - Certificate 📑

> Screenshot Navbar:  
> `docs/navbar.png` *(tambahkan screenshot setelah kamu ambil)*

---

### 2) Home (Hero Section)
**Fungsi:**
- Perkenalan singkat (nama, identitas, dan deskripsi miniproject)
- Menampilkan **minimal 1 gambar** (foto personal)

**Isi utama:**
- Judul: “Halo, Saya Dilla Maharani”
- Identitas singkat: jurusan, fakultas, universitas
- Paragraf perkenalan / miniproject
- Gambar pada sisi kanan

**Implementasi:**
- Section: `<section id="home">`
- Layout 2 kolom memakai flex:
  - kiri: `.teksperkenalan`
  - kanan: `.fotoku` + `<img>`

> Screenshot Home:  
> `docs/home.png`

---

### 3) About Me
Section ini memuat **3 bagian besar**: deskripsi, skills (progress bar), dan pengalaman (timeline).

#### a. Deskripsi Diri
**Fungsi:**
- Menjelaskan ringkas profil dan aktivitas

**Implementasi:**
- Container `.deskripsi` (background denim, text putih)

> Screenshot About - Deskripsi:  
> `docs/about-deskripsi.png`

#### b. Skills (Progress Bar)
**Fungsi:**
- Menampilkan hard skill & soft skill dalam bentuk progress bar

**Implementasi:**
- Dibagi 2 kolom:
  - `Hard Skill` (HTML, CSS, UI Design)
  - `Soft Skill` (Komunikasi, Kerja sama tim, Manajemen waktu)
- Progress bar dibuat dengan:
  - `.bar` sebagai track
  - `.fill` / `.fill2` sebagai isi bar
  - Lebar bar diatur inline `style="width:80%"` dll

> Screenshot About - Skills:  
> `docs/about-skills.png`

#### c. Pengalaman (Timeline)
**Fungsi:**
- Menampilkan pengalaman dalam format timeline agar rapi dan mudah dibaca

**Implementasi:**
- `.timeline` menggunakan pseudo element `::before` sebagai garis vertikal
- `.timeline-item::before` sebagai titik timeline
- Isi pengalaman meliputi judul, tahun/peran, dan deskripsi singkat

> Screenshot About - Pengalaman:  
> `docs/about-pengalaman.png`

---

### 4) Certificates (Card / Grid)
**Fungsi:**
- Menampilkan daftar sertifikat dalam bentuk **card** dan layout rapi

**Implementasi:**
- Section: `<section id="certificate">`
- Container `.sertif` menggunakan flex + gap
- Setiap sertifikat dibuat dengan **Bootstrap Card**:
  - `<div class="card custom-card">`
  - `<img class="card-img-top">`
  - `<div class="card-body">`

Contoh data sertifikat:
- INFORSA 2024
- INFORSA Mengabdi 2025
- MAKRAB SI 2024

> Screenshot Certificates:  
> `docs/certificates.png`

---

## 🎨 Penjelasan Styling (CSS)
Styling utama menggunakan file **style.css**, dengan konsep:
- **Palet warna** menggunakan CSS variable:
  - pink, denim, light, white, grey, dark
- Layout menggunakan **flexbox** agar tersusun rapi
- Tiap section dibuat full-height/min-height agar tampil seperti 1 halaman per section
- Progress bar custom untuk skill
- Card diberi radius agar terlihat modern

---

## 📌 Catatan Responsif
- Bootstrap 5 sudah terpasang via CDN untuk membantu komponen (card, utilities).
- Layout utama juga memakai flex CSS.
- Jika ingin lebih responsif di HP:
  - kamu bisa menambahkan `@media` di `style.css` untuk mengubah flex jadi column di layar kecil.

---

## 🖼️ Keseluruhan Gambar Tampilan Website (Wajib)
Tambahkan folder `docs/` berisi screenshot hasil tampilan:
- `docs/navbar.png`
- `docs/home.png`
- `docs/about-deskripsi.png`
- `docs/about-skills.png`
- `docs/about-pengalaman.png`
- `docs/certificates.png`
- (opsional) `docs/fullpage.png` (screenshot full page)

Cara ambil screenshot:
- Buka website di browser → gunakan screenshot tool (Snipping Tool / built-in screenshot) → simpan ke folder `docs/`.

---

## 👩🏻‍💻 Author
**Dilla Maharani**  
© 2026
