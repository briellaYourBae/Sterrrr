# Ruang Cerita Ester

Website pribadi Ester, mahasiswi Sistem Informasi di Universitas AMIKOM Yogyakarta.

Panduan ini menjelaskan cara **clone (menyalin) repository ke laptop** dan membuka websitenya. Clone hanya perlu dilakukan sekali di setiap laptop.

## 1. Pasang aplikasi yang dibutuhkan

### Git

Git digunakan untuk menyalin repository dari GitHub.

- **Windows:** unduh dan pasang Git dari [git-scm.com/download/win](https://git-scm.com/download/win). Saat instalasi, pilihan bawaan boleh digunakan.
- **macOS:** buka aplikasi Terminal dan ketik `git --version`. Jika Git belum tersedia, ikuti petunjuk instalasi yang muncul atau unduh Git dari [git-scm.com/download/mac](https://git-scm.com/download/mac).
- **Linux:** buka Terminal dan pasang Git melalui pengelola paket distro yang digunakan. Contoh untuk Ubuntu atau Debian: `sudo apt install git`.

Untuk memastikan Git sudah terpasang, buka **PowerShell** (Windows) atau **Terminal** (macOS/Linux), lalu jalankan:

```bash
git --version
```

Jika muncul nomor versi, misalnya `git version 2.x.x`, Git siap digunakan.

### Visual Studio Code (opsional)

Untuk mengedit file website, pasang [Visual Studio Code](https://code.visualstudio.com/). Untuk sekadar melihat website, browser seperti Chrome, Edge, atau Firefox sudah cukup.

## 2. Clone repository

1. Buka halaman repository: [github.com/briellaYourBae/Sterrrr](https://github.com/briellaYourBae/Sterrrr).
2. Tentukan lokasi untuk menyimpan folder website. Contohnya **Documents**.
3. Buka terminal di lokasi tersebut:
   - **Windows:** buka folder Documents di File Explorer, klik kanan area kosong, lalu pilih **Open in Terminal** atau **Open PowerShell window here**. Jika pilihan itu tidak tersedia, buka PowerShell dari menu Start, lalu pindah ke Documents dengan perintah:

     ```powershell
     cd "$HOME\Documents"
     ```

   - **macOS:** buka Terminal, lalu jalankan:

     ```bash
     cd ~/Documents
     ```

   - **Linux:** buka Terminal, lalu jalankan:

     ```bash
     cd ~/Documents
     ```

4. Salin perintah berikut, tempel ke terminal, lalu tekan **Enter**:

   ```bash
   git clone https://github.com/briellaYourBae/Sterrrr.git
   ```

5. Tunggu sampai proses selesai. Folder bernama `Sterrrr` akan dibuat di lokasi yang dipilih. Pastikan laptop terhubung ke internet.
6. Masuk ke folder repository:

   ```bash
   cd Sterrrr
   ```

Repository ini bisa di-clone tanpa login selama dapat diakses secara publik. Jangan mengetik tanda `$` atau `>` jika terminal menampilkannya sebelum perintah.

## 3. Buka website di browser

Setelah berada di dalam folder `Sterrrr`, buka file `index.html`:

- **Cara mudah:** buka folder `Sterrrr` di File Explorer (Windows) atau Finder (macOS), lalu klik dua kali `index.html`. Website akan terbuka di browser.
- **Lewat terminal:** jalankan perintah yang sesuai:

  **Windows PowerShell**

  ```powershell
  start index.html
  ```

  **macOS**

  ```bash
  open index.html
  ```

  **Linux**

  ```bash
  xdg-open index.html
  ```

Gunakan menu navigasi di website untuk membuka halaman Beranda, Aktivitas, Pendidikan, dan Jadwal Kuliah.

## 4. Buka dan edit di Visual Studio Code (opsional)

Jika Visual Studio Code sudah terpasang:

1. Buka Visual Studio Code.
2. Pilih **File → Open Folder...**.
3. Cari dan pilih folder `Sterrrr`, lalu klik **Select Folder** atau **Open**.
4. Di panel Explorer, klik file yang ingin dilihat atau diedit. Misalnya `index.html` atau `styles.css`.
5. Simpan perubahan dengan **Ctrl+S** (Windows/Linux) atau **Cmd+S** (macOS), lalu muat ulang halaman di browser.

Jika perintah `code .` sudah tersedia, folder juga dapat dibuka dari terminal dengan menjalankan perintah itu saat berada di dalam folder `Sterrrr`. Jika perintahnya tidak dikenali, gunakan cara **File → Open Folder...** di atas.

## 5. Mengambil perubahan terbaru

Jika repository di GitHub diperbarui dan kamu ingin mengambil versi terbaru:

1. Buka terminal di folder `Sterrrr`.
2. Jalankan:

   ```bash
   git pull
   ```

## Jika menemui masalah

- **`git` tidak dikenali:** Git belum terpasang, atau terminal perlu ditutup dan dibuka kembali setelah instalasi. Pasang Git lalu ulangi langkah clone.
- **Folder `Sterrrr` sudah ada:** jangan jalankan clone di lokasi yang sama untuk kedua kalinya. Buka folder yang sudah ada; untuk mengambil versi terbaru, jalankan `git pull` dari dalam folder itu.
- **Clone gagal atau koneksi terputus:** periksa koneksi internet dan pastikan alamat repository diketik persis seperti contoh.
- **Website tidak berubah setelah diedit:** simpan file, lalu muat ulang browser. Pastikan yang dibuka adalah `index.html` dari folder `Sterrrr`.

## Isi repository

- `index.html` — halaman beranda.
- `aktifitas.html` — halaman aktivitas.
- `pendidikan.html` — halaman pendidikan.
- `jadwal kuliah.html` — halaman jadwal kuliah.
- `styles.css` — gaya dan tata letak seluruh halaman.
