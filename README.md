# Vincent Alfian Artha – Digital Portfolio

Website portofolio digital modern, responsif, dan minimalis untuk menampilkan profil, skills, dan karya Project-Based Learning (PBL) serta Case-Based Learning (CBL).

## 📋 Deskripsi

Website ini dibuat sebagai portofolio pribadi dan tugas mata kuliah **Pengembangan Portofolio** di ITB STIKOM Bali. Website menampilkan:

- **Profil Diri**: Informasi lengkap tentang latar belakang pendidikan
- **Skills & Kompetensi**: Keahlian di bidang Web Development, Networking, dan IT Systems
- **Project-Based Learning (PBL)**: Sistem Informasi Booking Fasilitas Kampus
- **Case-Based Learning (CBL)**: Hotel Network Simulation & Routing with ACL
- **Kontak**: Form kontak dan informasi untuk berhubungan

## 🚀 Teknologi yang Digunakan

- **HTML5**: Struktur website
- **CSS3**: Styling dan desain responsif
- **JavaScript**: Interaktivitas dan animasi
- **Bootstrap 5**: Framework CSS untuk responsive design
- **Font Awesome**: Icon library
- **AOS (Animate On Scroll)**: Library animasi scroll
- **Google Fonts (Poppins)**: Typography

## 📁 Struktur Folder

```
my_digital_portfolio/
│
├── assets/
│   ├── css/
│   │   └── style.css          # File CSS utama
│   ├── js/
│   │   └── script.js          # File JavaScript utama
│   └── images/                # Folder untuk gambar (placeholder)
│
├── index.html                 # Halaman utama (Single Page Application)
└── README.md                  # Dokumentasi
```

## 🎨 Fitur Website

### 1. **Navigation Bar**
- Fixed navigation dengan smooth scrolling
- Active state berdasarkan section yang sedang dilihat
- Responsive mobile menu

### 2. **Hero Section**
- Desain modern dengan gradient background
- Social media links (GitHub, Email, LinkedIn)
- Call-to-action buttons

### 3. **About Me Section**
- Profil foto (placeholder)
- Informasi pendidikan lengkap
- Deskripsi singkat tentang diri

### 4. **Skills Section**
- Kategorisasi skills:
  - Programming & Web Development
  - Networking & Systems
  - Tools
- Icon-based skill cards dengan hover effect

### 5. **PBL Section**
- Detail proyek Sistem Informasi Booking Fasilitas Kampus
- Teknologi yang digunakan
- Fitur-fitur yang diimplementasikan
- Link ke GitHub repository

### 6. **CBL Section**
- Detail proyek Hotel Network Simulation
- Teknologi networking yang digunakan
- Hasil implementasi
- Link ke GitHub repository

### 7. **Contact Section**
- Informasi kontak (Email, GitHub, LinkedIn)
- Form kontak interaktif
- Validasi form sederhana

### 8. **Footer**
- Copyright information
- Social media links

## 💻 Cara Menjalankan Website

### Metode 1: Langsung Buka File HTML
1. Download atau clone repository ini
2. Buka file `index.html` dengan browser (Chrome, Firefox, Edge, dll)
3. Website akan langsung berjalan

### Metode 2: Menggunakan Live Server (Recommended)

#### Dengan VS Code:
1. Install extension **Live Server** di VS Code
2. Buka folder project di VS Code
3. Klik kanan pada `index.html`
4. Pilih **"Open with Live Server"**
5. Website akan terbuka di browser dengan auto-reload

#### Dengan XAMPP:
1. Copy folder `my_digital_portfolio` ke folder `htdocs` di XAMPP
2. Start Apache di XAMPP Control Panel
3. Buka browser dan akses: `http://localhost/my_digital_portfolio`

### Metode 3: Menggunakan Python Simple HTTP Server
```bash
# Masuk ke folder project
cd my_digital_portfolio

# Python 3
python -m http.server 8000

# Buka browser dan akses: http://localhost:8000
```

## 🌐 Deploy ke GitHub Pages

1. Push repository ke GitHub
2. Buka **Settings** repository
3. Pilih **Pages** di sidebar
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`
5. Klik **Save**
6. Website akan tersedia di: `https://username.github.io/repository-name`

## 📱 Responsive Design

Website ini fully responsive dan telah dioptimasi untuk berbagai ukuran layar:
- **Desktop**: 1200px ke atas
- **Tablet**: 768px - 1199px
- **Mobile**: 320px - 767px

## 🎯 Customization

### Mengganti Informasi Pribadi:
1. Buka `index.html`
2. Edit bagian yang sesuai (nama, email, deskripsi, dll)
3. Simpan dan refresh browser

### Mengganti Warna:
1. Buka `assets/css/style.css`
2. Edit CSS variables di bagian `:root`:
```css
:root {
    --primary-color: #4A90E2;  /* Warna utama */
    --secondary-color: #6C757D;
    /* ... */
}
```

### Menambahkan Gambar:
1. Simpan gambar di folder `assets/images/`
2. Update path di `index.html`:
```html
<img src="assets/images/nama-file.jpg" alt="Deskripsi">
```

## 📞 Kontak

- **Email**: vincentbocah@gmail.com
- **GitHub**: [@Vincentaa7](https://github.com/Vincentaa7)
- **LinkedIn**: [@Vincent Alfian Artha](https://www.linkedin.com/in/vincent-alfian-artha-0217032a0/)

## 📄 Lisensi

© 2025 Vincent Alfian Artha – Digital Portfolio. All rights reserved.

---

**Dibuat dengan ❤️ untuk tugas Pengembangan Portofolio - ITB STIKOM Bali**

