# Daftar Isi
  - [Proses Instalasi Apache2](#Proses-instalasi-Apache2)
# Apacahe2 And Tableau Installation
**Berikut adalah langkah-langkah menginstall Apache2 dan Tableau**!
# Proses instalasi Apache2
## 1. Instalasi Apache2 di Ubuntu Server
- Perbarui Paket Database Lokal
    ```bash
      sudo apt update
    ```

- Install Apache2
-  ```bash
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
-  ```bash
      sudo systemctl status apache2
    ```
      [cek status apache2](https://user-images.githubusercontent.com/150429308/282998909-8f1f021b-d09a-4ef8-9c8b-660908c43e92.png)

- Untuk mengecek bahwa Apache dapat berjalan dengan baik dapat menggunkan perintah
- - **Periksa Alamat IP**:
    ```bash
      hostname -I
    ```
    ![hostneme-I](https://user-images.githubusercontent.com/150429308/282998908-9947be4d-648f-4a07-9452-f62d03178295.png)

- Buka Broswer : Buka broswer yang berada di sistem operasi utama atau yang terhubung kejaringan yang sama 
-  Masukkan Alamat IP :Jika berhasil akan muncul halaman default Apache2

      ![tampilandefaultapache2](https://user-images.githubusercontent.com/150429308/282998906-39fcb4cc-fe1f-493a-9f7c-7ad2e0b762f8.png)

## 2. Membuat Halaman Web Sendiri

- Buat Direktori untuk Domain Anda
   ```bash
       sudo mkdir /var/www/html/nama_domain
    ```

  ![pemebuatan derektori baru](https://user-images.githubusercontent.com/150429308/282998903-12b66258-2eb1-4221-9236-e51d2a88c0e6.png)

- Buat dan Edit Laman Index HTML
   ```bash
        sudo nano /var/www/html/nama_domain/index.html
    ```
   ![pembuatan file direktori](https://user-images.githubusercontent.com/150429308/282998901-5732a827-57ba-48ce-8028-cd331f8e542a.png)

- Tambahkan kode HTML untuk tampilan halaman web sendiri
  Contoh kodingan
    ```bash
       <html>
    <head>
    <title>website YNTM</title>
    </head>
    <body>
    <h1>Selamat Datang di Website Diki Riskiyanto</h1>
    <from>
    <label> Nama: Diki Riskiyanto</label><br><br>
    <label> NIM : 0901128227111</label><br><br>
    <label> Kelas: SK5C<br><br>
    </body>
    </html>
    ```
- Simpan dan keluar dari editor

- Restart Apache2
   ```bash
      sudo systemctl restart apache2
    ```
   ![restart apache2](https://user-images.githubusercontent.com/150429308/282998898-743ee45b-ff89-4aa9-a5c5-2a32ba775e66.png)
- Masuk ke broswer masukan ip/nama_domain
  
![GAMABAR WEBSITE](https://user-images.githubusercontent.com/150429308/282998895-23f83576-e28e-4073-bffe-b1c1d7d62d4e.png)

## 3. Meremote Ubuntu Server

- Menggunakan PuTTY (di Windows):
  - Buka PuTTY, masukkan IP Ubuntu Server, atur connect type ke SSH, klik "Open".
    
![PUTTY](https://user-images.githubusercontent.com/150429308/282998894-c3559f54-6fa2-4e48-9f22-1fa7a97d3931.png)
  - Login dengan akun Ubuntu Server.

- Menggunakan Command Prompt (di Windows):
  - Ketikan di CMD
     ```bash
      sudo ssh user@ip_ubuntu_server
    ```
      ![WINDOWS](https://user-images.githubusercontent.com/150429308/282998892-e510e4a4-e9a9-41eb-89bb-c7732b801005.png)
  - Masukkan password akun Ubuntu Server

- Menggunakan Terminal (di Ubuntu):
  - Ketikan di terminal
      ```bash
      sudo ssh user@ip_ubuntu_server
    ```
  ![UBUNTU](https://user-images.githubusercontent.com/150429308/282998886-9135373c-31bc-4561-b1da-464291055c00.png)
  - Masukkan password akun Ubuntu Server
# Proses Instalisasi Tabluae
### Panduan Instalasi dan Visualisasi Data Menggunakan Tableau Public

1. **Instalasi Tableau Public**
   - Kunjungi website [Tableau Public](https://public.tableau.com/en-us/s/gallery) dan lakukan registrasi untuk membuat akun Tableau Public dengan mengisi data yang diminta.
   - Klik "Create My Account" dan verifikasi akun melalui email yang dikirimkan.
   - Setelah akun aktif, login ke Tableau Public.
   - Pada halaman utama setelah login, klik "Create" dan pilih "Download Tableau Desktop Public."
     
![create](https://github.com/dikiriskiyanto/Apacahe2-And-Tableau-Installation/assets/150429308/d172a283-c063-4314-8cde-5fe613c9c730)

   - Pilih sistem operasi yang sesuai dan lakukan instalasi.

2. **Membuat dan Menvisualisasikan Data di Tableau**
   - Hubungkan data dengan memilih jenis file, misalnya Microsoft Excel.
   - Pilih file yang akan diunggah dan buka.
   - Jika berhasil, tampilan data akan muncul.
   
![Gambar tampilan data](https://github.com/dikiriskiyanto/Apacahe2-And-Tableau-Installation/assets/150429308/3b89c4b4-191b-4471-8e11-960f6ea67d80)

   - Contoh data JUMLAH PULAU DI INDONESIA
   - Pilih "Sheet 1" untuk membuat visualisasi pertama. Tarik provinsi ke kolom, lalu pilih tampilan peta.
     
![sheet 1](https://github.com/dikiriskiyanto/Apacahe2-And-Tableau-Installation/assets/150429308/954b2b02-9f82-40e6-9de4-54d6da071919)

   - Masukkan data yang ingin ditampilkan di peta dengan menarik elemen data ke dalam gambar.
   - Buat sheet baru untuk membuat tabel jumlah pulau.
   - Tarik data provinsi ke kolom dan jumlah pulau ke baris.
   - Buat sheet baru lagi untuk menampilkan persentase wilayah.
   - Tarik data provinsi ke kolom dan persentase ke baris, pilih tampilan peta simbol.
   - Sesuaikan warna menggunakan opsi di menu warna.
     
![sheet 3](https://github.com/dikiriskiyanto/Apacahe2-And-Tableau-Installation/assets/150429308/cda5f4d5-e5de-4143-99d4-37bc7a511b74)

   - Buat dashboard dengan menambahkan sheet 1 ke dalamnya. Atur tata letak sesuai kebutuhan.

3. **Menyimpan dan Membagikan Hasil**
   - Setelah membuat dashboard, pindahkan ke depan untuk menampilkan hasilnya.
   - Untuk menyimpan hasil, klik "File" lalu pilih "Save to Tableau Public." Masukkan akun Tableau yang telah dibuat, beri nama file, dan simpan.
   - Anda akan diarahkan ke halaman web yang berisi tampilan data Tableau. Link tersebut dapat diakses oleh semua orang.
   - Karena ini versi public, hasilnya tidak dapat disimpan secara offline. Untuk menyimpan secara offline, instal versi berbayar seperti Tableau Desktop.

### Contoh Dashboard
![Contoh Dashboard](https://github.com/dikiriskiyanto/Install/blob/main/JUMLAH%20PULAU%20DI%20INDONESIA.png)

### Link Hasil Visualisasi
[Tableau Public - Jumlah Pulau di Indonesia Tahun 2021](https://public.tableau.com/app/profile/diki.riskiyanto/viz/JUMLAHPULAUDIINDONESIATAHUN2021/JUMLAHPULAUDIINDONESIA?publish=yes)

#UNTUK DETAIL PENGINSTALAN SILAKAN LIHAT LAPORAN 
