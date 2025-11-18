# 🎨 Panduan Customization Website

Dokumen ini berisi panduan lengkap untuk mengkustomisasi website portofolio Anda.

## 📝 Mengganti Informasi Pribadi

### 1. Nama dan Tagline (Hero Section)

Buka `index.html`, cari bagian Hero Section (sekitar baris 60-80):

```html
<h1 class="display-4 fw-bold mb-3">
    Hi, Saya <span class="text-primary">Vincent Alfian Artha</span>
</h1>
<h4 class="text-muted mb-4">Mahasiswa Sistem Komputer</h4>
<p class="lead mb-4">
    Web Development • Networking • IT Systems
</p>
```

Ganti dengan informasi Anda.

### 2. About Me Section

Cari bagian About (sekitar baris 100-150):

```html
<h3 class="mb-3">Vincent Alfian Artha</h3>
```

Ganti nama, program studi, kampus, dan deskripsi sesuai profil Anda.

### 3. Email dan Social Media

Cari semua link email dan social media:

```html
<!-- Email -->
<a href="mailto:your.email@example.com">

<!-- GitHub -->
<a href="https://github.com/Vincentaa7" target="_blank">

<!-- LinkedIn -->
<a href="#" target="_blank">
```

Ganti dengan link Anda yang sebenarnya.

## 🎨 Mengganti Warna Website

Buka `assets/css/style.css`, cari bagian `:root` (baris 10-20):

```css
:root {
    --primary-color: #4A90E2;      /* Warna utama (biru) */
    --secondary-color: #6C757D;    /* Warna sekunder (abu) */
    --success-color: #28A745;      /* Warna sukses (hijau) */
    --dark-color: #2C3E50;         /* Warna gelap */
    --light-color: #F8F9FA;        /* Warna terang */
}
```

### Contoh Skema Warna Alternatif:

**Purple Theme:**
```css
--primary-color: #9B59B6;
--success-color: #8E44AD;
```

**Orange Theme:**
```css
--primary-color: #E67E22;
--success-color: #D35400;
```

**Green Theme:**
```css
--primary-color: #27AE60;
--success-color: #229954;
```

## 🖼️ Mengganti Gambar

### 1. Foto Profil

1. Siapkan foto Anda (format: JPG/PNG, ukuran: 500x500px recommended)
2. Rename menjadi `profile.jpg`
3. Copy ke folder `assets/images/`
4. Buka `index.html`, cari:
   ```html
   <img src="assets/images/profile-placeholder.jpg" alt="Vincent Alfian Artha">
   ```
5. Ganti menjadi:
   ```html
   <img src="assets/images/profile.jpg" alt="Nama Anda">
   ```

### 2. Hero Illustration

Sama seperti foto profil, ganti file `hero-illustration.svg` dengan gambar Anda.

## 📚 Mengganti Konten Project

### Project PBL

Buka `index.html`, cari section `id="pbl"` (sekitar baris 380-470):

```html
<h3 class="project-title">Sistem Informasi Booking Fasilitas Kampus</h3>
```

Ganti:
- Judul project
- Deskripsi tujuan
- Teknologi yang digunakan
- Hasil & fitur
- Link GitHub

### Project CBL

Sama seperti PBL, cari section `id="cbl"` dan ganti kontennya.

## 🔧 Menambah/Mengurangi Skills

Buka `index.html`, cari section `id="skills"`:

### Menambah Skill Baru:

Copy-paste block ini dan sesuaikan:

```html
<div class="col-lg-2 col-md-4 col-6 mb-4" data-aos="zoom-in" data-aos-delay="100">
    <div class="skill-card">
        <i class="fab fa-react"></i>  <!-- Ganti icon -->
        <p>React</p>                   <!-- Ganti nama skill -->
    </div>
</div>
```

### Icon Font Awesome:

Cari icon di: [Font Awesome Icons](https://fontawesome.com/icons)

Contoh:
- `fab fa-react` - React
- `fab fa-python` - Python
- `fab fa-docker` - Docker
- `fas fa-database` - Database

## 📱 Mengganti Font

Buka `index.html`, cari bagian `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

Ganti `Poppins` dengan font lain dari [Google Fonts](https://fonts.google.com/):
- Inter
- Roboto
- Montserrat
- Open Sans

Lalu di `assets/css/style.css`, ganti:

```css
body {
    font-family: 'Poppins', sans-serif;
}
```

## 🎭 Menambah Section Baru

### Contoh: Menambah Section "Sertifikat"

1. Buka `index.html`
2. Tambahkan di navigation:
   ```html
   <li class="nav-item">
       <a class="nav-link" href="#certificates">Sertifikat</a>
   </li>
   ```

3. Tambahkan section baru sebelum Contact:
   ```html
   <section id="certificates" class="section-padding bg-light">
       <div class="container">
           <div class="row">
               <div class="col-lg-12 text-center mb-5" data-aos="fade-up">
                   <h2 class="section-title">Sertifikat</h2>
                   <div class="title-underline"></div>
               </div>
           </div>
           <!-- Konten sertifikat di sini -->
       </div>
   </section>
   ```

## 🔄 Menonaktifkan Animasi

Jika Anda ingin website tanpa animasi:

1. Buka `index.html`
2. Hapus/comment baris ini:
   ```html
   <!-- <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet"> -->
   <!-- <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script> -->
   ```

3. Hapus semua atribut `data-aos` di HTML

## 📊 Menambah Google Analytics

1. Daftar di [Google Analytics](https://analytics.google.com)
2. Dapatkan Tracking ID (format: G-XXXXXXXXXX)
3. Tambahkan di `<head>` sebelum `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🎯 Tips Customization

1. **Backup**: Selalu backup file sebelum edit
2. **Test**: Test setiap perubahan di browser
3. **Responsive**: Cek tampilan di mobile setelah edit
4. **Konsisten**: Gunakan warna dan font yang konsisten
5. **Simple**: Jangan terlalu banyak animasi/efek

## 🆘 Troubleshooting

### Perubahan tidak muncul?
- Hard refresh browser: `Ctrl + F5` (Windows) atau `Cmd + Shift + R` (Mac)
- Clear browser cache
- Cek apakah file sudah tersimpan

### Layout berantakan?
- Cek apakah ada tag HTML yang tidak tertutup
- Pastikan tidak menghapus class Bootstrap
- Validasi HTML di [W3C Validator](https://validator.w3.org/)

### Warna tidak berubah?
- Pastikan edit di file `style.css` yang benar
- Cek apakah ada `!important` yang override
- Clear cache browser

---

**Selamat berkreasi! 🎨**

Jika ada pertanyaan, silakan buka issue di GitHub repository.

