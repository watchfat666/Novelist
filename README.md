[README.md](https://github.com/user-attachments/files/29515728/README.md)
# Novelist# Pena — Studio Penulisan Novel

Website satu-file (HTML/CSS/JS) untuk menulis novel: cerita, plot, adegan, dialog, dan karakter — lengkap dengan tooltip gambar karakter saat nama karakter disebut di teks mana pun.

## Cara mempublikasikan di GitHub Pages (gratis, tanpa server)

1. Buat repository baru di GitHub, misalnya `novel-app`.
2. Unggah file `index.html` ini ke root repository (drag & drop lewat tombol "Add file" → "Upload files" di GitHub, atau lewat `git push`).
3. Buka tab **Settings** → **Pages** di repository.
4. Pada bagian **Build and deployment**, pilih source: **Deploy from a branch**, branch: `main`, folder: `/ (root)`. Klik **Save**.
5. Tunggu 1-2 menit, lalu situs akan tersedia di:
   `https://<username-github-kamu>.github.io/novel-app/`

## Cara kerja & catatan penting

- **Tanpa server/backend** — semua data (cerita, karakter, plot, adegan, dialog) disimpan di `localStorage` browser kamu. Artinya data hanya tersimpan di perangkat dan browser yang sama; tidak otomatis sinkron antar perangkat.
- **Cadangkan data**: di tab "Ringkasan Cerita" ada tombol **Ekspor JSON** untuk mengunduh data cerita sebagai cadangan.
- **Gambar karakter**: bisa berupa URL gambar online, atau unggah file gambar langsung (disimpan sebagai data di browser).
- **Deteksi nama karakter**: setiap kali nama karakter (persis sesuai yang diinput) muncul di sinopsis cerita, plot, adegan, atau dialog, nama itu otomatis ditandai. Arahkan kursor (hover) ke nama tersebut untuk melihat gambar dan deskripsi karakter.

## Mengembangkan lebih lanjut

Jika nanti ingin data tersimpan di cloud (sinkron antar perangkat, multi-pengguna), langkah berikutnya adalah menambahkan backend sederhana, misalnya Firebase, Supabase, atau GitHub sebagai penyimpanan lewat GitHub API/Issues. Beri tahu saya jika kamu ingin saya bantu menambahkan itu.
