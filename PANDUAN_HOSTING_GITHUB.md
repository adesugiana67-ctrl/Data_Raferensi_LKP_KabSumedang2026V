# Panduan Hosting Github Pages - SIPNF Kabupaten Sumedang

Aplikasi **Sistem Informasi & Pelaporan Pendidikan Non Formal (SIPNF) Kabupaten Sumedang** dirancang sebagai *Single Page Application (SPA)* berbasis peramban (client-side) lengkap dengan penyimpanan lokal interaktif (`localStorage`).

Sistem ini telah dikonfigurasi menggunakan plugin `vite-plugin-singlefile` yang menggabungkan seluruh komponen React, Tailwind CSS, dan ikon Lucide ke dalam satu file HTML mandiri (bundle tunggal).

## 📁 Lokasi File HTML untuk Hosting Github
File HTML siap hosting berada pada jalur berikut di repositori/proyek ini:
- **`dist/index.html`** (File utama hasil build otomatis yang berukuran sekitar 322 KB).

---

## 🚀 Langkah-Langkah Publikasi ke GitHub Pages (100% Gratis)

### Langkah 1: Buat Repositori GitHub
1. Buka akun [GitHub](https://github.com) Anda.
2. Buat repositori baru (klik tombol **New**).
3. Beri nama repositori, contoh: `sipnf-sumedang` atau `pelaporan-pnf-sumedang`.
4. Pilih visibilitas **Public**.
5. Klik **Create repository**.

### Langkah 2: Unggah File HTML
Anda memiliki 2 opsi mudah untuk mengunggah file HTML:

#### Opsi A: Cara Manual via Web GitHub (Sangat Disarankan bagi Pemula)
1. Buka halaman repositori GitHub yang baru saja Anda buat.
2. Klik link **"uploading an existing file"**.
3. Buka folder `dist` pada komputer Anda, kemudian seret (drag & drop) file `index.html` yang berada di dalam folder `dist` tersebut ke halaman GitHub.
4. Klik **Commit changes**.

#### Opsi B: Cara via Git Terminal / Git CLI
```bash
# Inisialisasi git di dalam folder dist
cd dist
git init
git checkout -b main
git add .
git commit -m "Deploy SIPNF Sumedang ke Github Pages"
git remote add origin https://github.com/username-anda/sipnf-sumedang.git
git push -u origin main
```

### Langkah 3: Aktifkan Fitur GitHub Pages
1. Pada halaman repositori GitHub Anda, klik tab ⚙️ **Settings**.
2. Pada menu di bilah sebelah kiri, pilih **Pages** (berada di bawah kategori *Code and automation*).
3. Pada bagian **Build and deployment**:
   - **Source**: Pilih `Deploy from a branch`.
   - **Branch**: Pilih `main` (atau `master`), lalu pilih folder `/ (root)`.
4. Klik tombol **Save**.

### Langkah 4: Website Selesai dan Live!
1. Tunggu sekitar 1–3 menit hingga GitHub memproses halaman Anda.
2. Di bagian atas halaman pengaturan *Pages* tadi, akan muncul tautan web Anda, seperti:
   👉 `https://username-anda.github.io/sipnf-sumedang/`
3. Aplikasi web pelaporan dua arah Kabupaten Sumedang Anda siap diakses oleh masyarakat, operator sekolah, dan admin dinas pendidikan!

---

## 💡 Fitur Unggulan dalam File HTML Ini:
- **Akses Offline/Penyimpanan Lokal:** Perubahan data pada form pendaftaran sekolah, SPMB, dan raport otomatis disimpan di memori browser pengguna.
- **Responsive 100%:** Siap diakses melalui perangkat seluler (HP) maupun Desktop/Laptop.
- **Pergantian Peran Instan:** Penguji/pengawas Disdik Sumedang dapat langsung beralih peran ke mode **Dinas / Verifikator** untuk menyetujui ajukan dan memberi umpan balik.
