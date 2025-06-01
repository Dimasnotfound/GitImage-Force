# GitImage-Force

**GitImage-Force** adalah aplikasi web sederhana yang memungkinkan Anda mengunggah gambar ke repositori GitHub Anda melalui antarmuka grafis. Aplikasi ini memanfaatkan GitHub API untuk menyimpan gambar dan memberikan URL langsung beserta sintaks Markdown untuk digunakan di README.md atau dokumentasi lainnya.

## 🚀 Fitur

- Upload gambar ke repositori GitHub dengan mudah
- Preview gambar sebelum diunggah
- Mendapatkan URL langsung dan format Markdown untuk gambar
- Tidak perlu install—cukup buka di browser

## 🖼️ Demo Antarmuka

![preview](https://user-images.githubusercontent.com/your-username/sample-demo.png) <!-- Ganti dengan tangkapan layar aktual bila ada -->

## 📦 Cara Menggunakan

1. **Dapatkan Personal Access Token GitHub**  
   - Kunjungi [GitHub Settings > Developer Settings > Tokens](https://github.com/settings/tokens)
   - Buat token baru dengan scope `repo`

2. **Masukkan Informasi di Aplikasi**
   - Masukkan **GitHub Token**
   - Masukkan **Nama Repositori** dalam format `username/repo`
   - Pilih **gambar** yang ingin diunggah

3. **Klik "Upload Image"**
   - Setelah sukses, URL gambar dan Markdown akan muncul

## 📁 Struktur Upload

Gambar akan diunggah ke folder `images/` dalam repositori yang Anda tentukan. Contoh:
```
https://github.com/username/repo/blob/main/images/your-image.png
```

## 📄 Contoh Markdown

Setelah upload berhasil, Anda akan mendapatkan format seperti:
```md
![your-image.png](https://raw.githubusercontent.com/username/repo/main/images/your-image.png)
```

## 🛡️ Keamanan

- Token Anda **tidak disimpan** atau dikirim ke pihak ketiga
- Pastikan untuk **menghapus** token setelah selesai, atau **gunakan token dengan akses terbatas**

## 🧪 Teknologi

- HTML5
- JavaScript (Vanilla)
- [GitHub REST API v3](https://docs.github.com/en/rest)
- TailwindCSS

## 📂 Cara Menjalankan Secara Lokal

Cukup buka file `index.html` di browser:

```bash
git clone https://github.com/your-username/gitimage-force.git
cd gitimage-force
open index.html # atau buka manual di browser
```

## ✅ TODO (Pengembangan Selanjutnya)

- Simpan daftar gambar yang telah diunggah
- Tambahkan opsi pengaturan cabang selain `main`
- Dukungan untuk drag-and-drop

## 📝 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).