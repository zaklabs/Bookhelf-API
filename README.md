# Bookshelf API

Proyek ini adalah submission untuk kelas **Belajar Membuat Aplikasi Back-End untuk Pemula** di Dicoding. API ini dibangun untuk mengelola data buku pada sebuah rak buku (bookshelf) virtual.

## Fitur Utama & Kriteria yang Terpenuhi
Aplikasi ini telah memenuhi seluruh kriteria wajib (mandatory) dan opsional (optional) yang disyaratkan:
- **Kriteria 1:** Aplikasi menggunakan port `9000`.
- **Kriteria 2:** Aplikasi dijalankan dengan perintah `npm run start` (serta `npm run start-dev` menggunakan nodemon untuk development).
- **Kriteria 3:** API dapat menyimpan buku (`POST /books`).
- **Kriteria 4:** API dapat menampilkan seluruh buku (`GET /books`).
- **Kriteria 5:** API dapat menampilkan detail buku (`GET /books/{bookId}`).
- **Kriteria 6:** API dapat mengubah data buku (`PUT /books/{bookId}`).
- **Kriteria 7:** API dapat menghapus buku (`DELETE /books/{bookId}`).
- **Opsional 1:** Mendukung fitur query parameters pada route `GET /books` (`?name`, `?reading`, `?finished`).
- **Opsional 2:** Menggunakan **ESLint** agar gaya penulisan kode JavaScript konsisten dan terhindar dari error.

## Teknologi yang Digunakan
- **Node.js** (Runtime Environment)
- **@hapi/hapi** (Web Framework)
- **nanoid** (ID Generator)
- **ESLint** (Linter / Code Quality)
- **Nodemon** (Development Monitor)

## Cara Menjalankan Aplikasi Secara Lokal

1. **Pastikan Anda memiliki Node.js terinstal di sistem Anda.**
2. **Kloning atau unduh repository ini.**
3. **Masuk ke folder proyek:**
   ```bash
   cd BookshelfAPI
   ```
4. **Instal seluruh dependensi yang dibutuhkan:**
   ```bash
   npm install
   ```
5. **Jalankan aplikasi:**
   - Untuk mode produksi:
     ```bash
     npm run start
     ```
   - Untuk mode pengembangan (auto-restart saat ada perubahan kode):
     ```bash
     npm run start-dev
     ```
6. **Server akan berjalan di:** `http://localhost:9000`

## Menjalankan Linter
Untuk memeriksa apakah ada kode yang tidak sesuai dengan *style guide* yang diterapkan, jalankan perintah berikut:
```bash
npm run lint
```

## Pengujian dengan Postman
Proyek ini dapat diuji menggunakan Postman Collection dan Environment yang disediakan oleh Dicoding (berada dalam direktori proyek ini). Anda bisa menjalankannya via aplikasi Postman secara manual, atau menggunakan `newman`:
```bash
npx newman run "Bookshelf API Test.postman_collection.json" -e "Bookshelf API Test.postman_environment.json"
```
*(Seluruh tes mandatory dan opsional dilaporkan lulus pengujian 100%).*
