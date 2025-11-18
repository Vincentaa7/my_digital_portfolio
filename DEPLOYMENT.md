# 🚀 Panduan Deployment ke GitHub Pages

Dokumen ini berisi langkah-langkah lengkap untuk mempublikasikan website portofolio Anda ke GitHub Pages.

## 📋 Prasyarat

- Akun GitHub (gratis)
- Git terinstall di komputer
- Repository GitHub (baru atau existing)

## 🔧 Langkah 1: Persiapan Repository

### A. Membuat Repository Baru di GitHub

1. Login ke [GitHub](https://github.com)
2. Klik tombol **"New"** atau **"+"** di pojok kanan atas
3. Pilih **"New repository"**
4. Isi informasi repository:
   - **Repository name**: `my-digital-portfolio` (atau nama lain)
   - **Description**: "Website Portofolio Digital - Vincent Alfian Artha"
   - **Public** (agar bisa di-deploy ke GitHub Pages gratis)
   - ✅ Centang **"Add a README file"** (opsional, karena sudah ada)
5. Klik **"Create repository"**

### B. Menghubungkan Project Lokal dengan GitHub

Buka terminal/command prompt di folder project, lalu jalankan:

```bash
# Inisialisasi Git (jika belum)
git init

# Tambahkan semua file
git add .

# Commit pertama
git commit -m "Initial commit: Portfolio website"

# Tambahkan remote repository (ganti URL dengan repository Anda)
git remote add origin https://github.com/Vincentaa7/my-digital-portfolio.git

# Push ke GitHub
git branch -M main
git push -u origin main
```

## 🌐 Langkah 2: Aktivasi GitHub Pages

1. Buka repository Anda di GitHub
2. Klik tab **"Settings"** (⚙️)
3. Scroll ke bawah dan klik **"Pages"** di sidebar kiri
4. Di bagian **"Source"**:
   - Branch: Pilih **`main`**
   - Folder: Pilih **`/ (root)`**
5. Klik **"Save"**
6. Tunggu beberapa saat (1-2 menit)
7. Refresh halaman, akan muncul link website Anda:
   ```
   https://vincentaa7.github.io/my-digital-portfolio/
   ```

## ✅ Langkah 3: Verifikasi Deployment

1. Klik link yang muncul di GitHub Pages settings
2. Website Anda seharusnya sudah live!
3. Jika ada error, cek:
   - Pastikan file `index.html` ada di root folder
   - Pastikan semua path file (CSS, JS, images) menggunakan relative path
   - Cek browser console untuk error

## 🔄 Update Website

Setiap kali Anda melakukan perubahan:

```bash
# Tambahkan file yang diubah
git add .

# Commit dengan pesan yang jelas
git commit -m "Update: Deskripsi perubahan"

# Push ke GitHub
git push origin main
```

GitHub Pages akan otomatis update dalam 1-2 menit.

## 🎨 Custom Domain (Opsional)

Jika Anda memiliki domain sendiri (misal: `vincentalfian.com`):

1. Beli domain dari provider (Niagahoster, Hostinger, dll)
2. Di GitHub Pages settings, masukkan domain di **"Custom domain"**
3. Di DNS provider, tambahkan CNAME record:
   ```
   Type: CNAME
   Name: www
   Value: vincentaa7.github.io
   ```
4. Tunggu propagasi DNS (bisa 24-48 jam)

## 🔒 HTTPS

GitHub Pages otomatis menyediakan HTTPS. Pastikan:
- ✅ Centang **"Enforce HTTPS"** di GitHub Pages settings

## 📱 Testing

Setelah deploy, test website di:
- Desktop (Chrome, Firefox, Edge)
- Mobile (responsive view)
- Tablet

Tools untuk testing:
- [Google Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)
- [PageSpeed Insights](https://pagespeed.web.dev/)

## 🐛 Troubleshooting

### Website tidak muncul
- Pastikan repository **Public**
- Pastikan file `index.html` ada di root
- Tunggu 5-10 menit setelah aktivasi

### CSS/JS tidak load
- Cek path file (harus relative, bukan absolute)
- Contoh benar: `assets/css/style.css`
- Contoh salah: `/assets/css/style.css` atau `C:/xampp/...`

### Gambar tidak muncul
- Pastikan gambar ada di folder `assets/images/`
- Cek case-sensitive (Linux server case-sensitive)
- Gunakan format yang didukung: JPG, PNG, SVG, GIF

## 📊 Analytics (Opsional)

Tambahkan Google Analytics untuk tracking visitor:

1. Daftar di [Google Analytics](https://analytics.google.com)
2. Dapatkan tracking code
3. Tambahkan di `<head>` file `index.html`

## 🎯 SEO Optimization

Untuk meningkatkan visibility di search engine:

1. **Meta Tags** (sudah ada di `index.html`):
   ```html
   <meta name="description" content="...">
   <meta name="keywords" content="...">
   ```

2. **Sitemap**: Buat file `sitemap.xml` (opsional untuk single page)

3. **robots.txt**: Buat file `robots.txt` di root:
   ```
   User-agent: *
   Allow: /
   ```

## 📞 Support

Jika ada masalah:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Community](https://github.community/)

---

**Selamat! Website portofolio Anda sudah online! 🎉**

Share link Anda di:
- LinkedIn
- Instagram
- CV/Resume
- Email signature

