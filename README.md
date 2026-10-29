# Nanas-Project

Repository data sumber (JSON API) publik untuk menampilkan daftar portofolio proyek (Website dan Aplikasi) pada website personal **Adnan Ferdiansyah (Nanas)**.

Data ini diakses langsung oleh front-end melalui GitHub Raw Content URL:
- **Kategori Website**: `https://raw.githubusercontent.com/nanasmuda121/Nanas-Project/main/website.json`
- **Kategori Aplikasi**: `https://raw.githubusercontent.com/nanasmuda121/Nanas-Project/main/aplikasi.json`

---

## Struktur File JSON

Setiap file (`website.json` & `aplikasi.json`) berisi array objek dengan format berikut:

```json
[
  {
    "id": 1,
    "judul": "Nama Project",
    "subjudul": "Subjudul project",
    "deskripsi": "Deskripsi singkat project",
    "tags": ["React", "Tailwind"],
    "image_url": "https://images.unsplash.com/photo-xxx"
  }
]
```

### Keterangan Field:
| Field | Tipe Data | Deskripsi |
|---|---|---|
| `id` | number | ID unik project (angka increment) |
| `judul` | string | Nama utama proyek |
| `subjudul` | string | Kategori / peran / tagline singkat |
| `deskripsi` | string | Penjelasan singkat fitur dan tujuan proyek |
| `tags` | string[] | Array teknologi / framework yang digunakan |
| `image_url` | string | URL gambar banner / thumbnail proyek |

---

## Cara Menambah / Mengubah Data Project

1. Buka file yang ingin diubah di GitHub:
   - Untuk proyek web: buka [`website.json`](website.json)
   - Untuk proyek aplikasi: buka [`aplikasi.json`](aplikasi.json)
2. Klik tombol **Edit this file** (ikon pensil 📝 di pojok kanan atas file).
3. Tambahkan objek JSON baru di dalam array. Contoh:
   ```json
   {
     "id": 4,
     "judul": "Proyek Keren Baru",
     "subjudul": "Full-stack Platform",
     "deskripsi": "Platform modern dengan arsitektur scalable.",
     "tags": ["Next.js", "TypeScript", "Tailwind CSS"],
     "image_url": "https://images.unsplash.com/photo-..."
   }
   ```
4. Pastikan tanda koma (`,`) antar elemen objek terpasang dengan benar dan tidak ada koma di item terakhir (*trailing comma*).
5. Tulis pesan commit (misal: `feat: tambah proyek baru`) lalu klik **Commit changes**.
6. Perubahan akan otomatis langsung aktif dan muncul di website portofolio!
