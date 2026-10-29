# Nanas-Project

Repository data sumber (JSON API) publik untuk menampilkan daftar portofolio proyek (Website dan Aplikasi) serta statistik pengalaman pada website personal **Adnan Ferdiansyah (Nanas)**.

Data ini diakses langsung oleh front-end melalui GitHub Raw Content URL:
- **Kategori Website**: `https://raw.githubusercontent.com/nanasmuda121/Nanas-Project/main/website.json`
- **Kategori Aplikasi**: `https://raw.githubusercontent.com/nanasmuda121/Nanas-Project/main/aplikasi.json`
- **Statistik Pengalaman**: `https://raw.githubusercontent.com/nanasmuda121/Nanas-Project/main/pengalaman.json`

---

## 1. Struktur File Proyek (`website.json` & `aplikasi.json`)

Setiap file berisi array objek proyek:

```json
[
  {
    "id": 1,
    "judul": "Nama Project",
    "subjudul": "Subjudul project",
    "deskripsi": "Deskripsi singkat project",
    "tags": ["React", "Tailwind"],
    "image_url": "https://images.unsplash.com/photo-xxx",
    "link_url": "https://nama-project.com"
  }
]
```

### Keterangan Field Proyek:
| Field | Tipe Data | Deskripsi |
|---|---|---|
| `id` | number | ID unik project (angka increment) |
| `judul` | string | Nama utama proyek |
| `subjudul` | string | Kategori / peran / tagline singkat |
| `deskripsi` | string | Penjelasan singkat fitur dan tujuan proyek |
| `tags` | string[] | Array teknologi / framework yang digunakan |
| `image_url` | string | URL gambar thumbnail / banner proyek |
| `link_url` | string | URL tautan live demo / situs web / repository proyek (bisa diklik) |

---

## 2. Struktur File Statistik (`pengalaman.json`)

File `pengalaman.json` mengatur angka statistik pengalaman yang tampil di halaman `/project/`:

```json
[
  {
    "id": "pengalaman",
    "value": 3,
    "suffix": "+",
    "label": "Tahun Pengalaman",
    "deskripsi": "Pengalaman belajar dan membangun berbagai solusi web & aplikasi interaktif."
  },
  {
    "id": "proyek",
    "value": 15,
    "suffix": "+",
    "label": "Proyek Selesai",
    "deskripsi": "Aplikasi web responsif, antarmuka visual, dan sistem perangkat lunak modern."
  },
  {
    "id": "teknologi",
    "value": 12,
    "suffix": "+",
    "label": "Teknologi Dikuasai",
    "deskripsi": "React, TypeScript, Tailwind CSS, Vite, Framer Motion, Node.js, dan 3D visual."
  }
]
```

---

## 3. Cara Menambah / Mengubah Data

1. Buka file yang ingin diubah di GitHub:
   - Proyek website: [`website.json`](website.json)
   - Proyek aplikasi: [`aplikasi.json`](aplikasi.json)
   - Statistik pengalaman: [`pengalaman.json`](pengalaman.json)
2. Klik tombol **Edit this file** (ikon pensil 📝).
3. Lakukan pengeditan data.
4. Klik **Commit changes**.
5. Website portofolio akan langsung memperbarui tampilan secara otomatis!
