# Apacahe2 And Tableau Installation
**Berikut adalah langkah-langkah menginstall Apache2 dan Tableau**!
# Daftar Isi
# Proses instalisai Apache2
## 1. Instalasi Apache2 di Ubuntu Server
- Perbarui Paket Database Lokal
    ```bash
      sudo apt update
    ```

- Install Apache2
   ```
  sudo apt install apache2
     ```
- Izinkan Apache Melalui Firewall:
    ```bash
      sudo ufw allow 'Apache'
    ```
- Aktifkan UFW:
    ```bash
      sudo ufw enable
    ```
- Periksa Status Apache2
     ```
  sudo systemctl status apache2
     ```
- Untuk mengecek bahwa Apache dapat berjalan dengan baik dapat menggunkan perintah
- - **Periksa Alamat IP**:
    ```bash
      hostname -I
    ```
- Buka Broswer : Buka broswer yang berada di sistem operasi utama atau yang terhubung kejaringan yang sama 
-  Masukkan Alamat IP :
  Jika berhasil akan muncul halaman default Apache2
## 2. Membuat Halaman Web Sendiri

- Buat Direktori untuk Domain Anda
   ```
   sudo mkdir /var/www/html/nama_domain
- Buat dan Edit Laman Index HTML
   ```
   sudo nano /var/www/html/nama_domain/index.html
   
- Tambahkan kode HTML untuk tampilan halaman web sendiri
- Simpan dan keluar dari editor

- Restart Apache2
   ```
   sudo systemctl restart apache2
   
## 3. Meremote Ubuntu Server

- Menggunakan PuTTY (di Windows):
  - Buka PuTTY, masukkan IP Ubuntu Server, atur connect type ke SSH, klik "Open".
  - Login dengan akun Ubuntu Server.

- Menggunakan Command Prompt (di Windows):
  - Ketikan di CMD 
     ```
     sudo ssh user@ip_ubuntu_server
        
  - Masukkan password akun Ubuntu Server

- Menggunakan Terminal (di Ubuntu):
  - Ketikan di terminal
     ```
     sudo ssh user@ip_ubuntu_server
     
  - Masukkan password akun Ubuntu Server
# Proses Instalisasi Tabluae
### Panduan Instalasi dan Visualisasi Data Menggunakan Tableau Public

1. **Instalasi Tableau Public**
   - Kunjungi website [Tableau Public](https://public.tableau.com/en-us/s/gallery) dan lakukan registrasi untuk membuat akun Tableau Public dengan mengisi data yang diminta.
   - Klik "Create My Account" dan verifikasi akun melalui email yang dikirimkan.
   - Setelah akun aktif, login ke Tableau Public.
   - Pada halaman utama setelah login, klik "Create" dan pilih "Download Tableau Desktop Public."
   - Pilih sistem operasi yang sesuai dan lakukan instalasi.

2. **Membuat dan Menvisualisasikan Data di Tableau**
   - Hubungkan data dengan memilih jenis file, misalnya Microsoft Excel.
   - Pilih file yang akan diunggah dan buka.
   - Jika berhasil, tampilan data akan muncul.
   - Pilih "Sheet 1" untuk membuat visualisasi pertama. Tarik provinsi ke kolom, lalu pilih tampilan peta.
   - Masukkan data yang ingin ditampilkan di peta dengan menarik elemen data ke dalam gambar.
   - Buat sheet baru untuk membuat tabel jumlah pulau.
   - Tarik data provinsi ke kolom dan jumlah pulau ke baris.
   - Buat sheet baru lagi untuk menampilkan persentase wilayah.
   - Tarik data provinsi ke kolom dan persentase ke baris, pilih tampilan peta simbol.
   - Sesuaikan warna menggunakan opsi di menu warna.
   - Buat dashboard dengan menambahkan sheet 1 ke dalamnya. Atur tata letak sesuai kebutuhan.

3. **Menyimpan dan Membagikan Hasil**
   - Setelah membuat dashboard, pindahkan ke depan untuk menampilkan hasilnya.
   - Untuk menyimpan hasil, klik "File" lalu pilih "Save to Tableau Public." Masukkan akun Tableau yang telah dibuat, beri nama file, dan simpan.
   - Anda akan diarahkan ke halaman web yang berisi tampilan data Tableau. Link tersebut dapat diakses oleh semua orang.
   - Karena ini versi public, hasilnya tidak dapat disimpan secara offline. Untuk menyimpan secara offline, instal versi berbayar seperti Tableau Desktop.

### Contoh Dashboard
![Contoh Dashboard](https://www.dropbox.com/scl/fi/fu1p490mk0fh8fyqgo3k6/JUMLAH-PULAU-DI-INDONESIA.png?rlkey=79xnbkigqbpoi736aj2c4do9o&dl=0)

### Link Hasil Visualisasi
[Tableau Public - Jumlah Pulau di Indonesia Tahun 2021](https://public.tableau.com/app/profile/diki.riskiyanto/viz/JUMLAHPULAUDIINDONESIATAHUN2021/JUMLAHPULAUDIINDONESIA?publish=yes)

Jika ada pertanyaan atau perlu bantuan lebih lanjut, jangan ragu untuk menghubungi saya.
