# Lab7Web_PHP
Laporan Praktikum 7

1. Tujuan Praktikum

Tujuan dari praktikum ini adalah mempelajari dasar-dasar pemrograman PHP dan memahami bagaimana PHP digunakan untuk mengolah data pada sebuah website.
Adapun tujuan khusus dari praktikum ini adalah :
1.Memahami cara menjalankan PHP menggunakan web server lokal.
2.Mempelajari penggunaan variabel dan perintah echo.
3.Memahami penggunaan kondisi if, elseif, dan else
4.Mempelajari penggunaan array dan foreach.
5.Membuat function untuk melakukan perhitungan dan menentukan kelulusan.
6.Memahami penggunaan metode GET dan POST pada formulir.
7.Mempelajari cara memproses dan memvalidasi data pengguna.
8.Memahami penggunaan htmlspecialchars() untuk mengamankan output.
9.Membuat aplikasi formulir data mahasiswa menggunakan PHP.

2. Perangkat yang Digunakan
Perangkat yang digunakan dalam praktikum ini adalah :
Laptop/Komputer : Digunakan untuk menjalankan program.
XAMPP : Digunakan sebagai web server lokal untuk menjalankan PHP.
Visual Studio Code : Digunakan untuk menulis dan mengedit kode program PHP.
Google Chrome : Digunakan untuk membuka dan melihat hasil program.
Windows : Sistem operasi yang digunakan.

3. Cara Menjalankan Server Lokal
Berikut langkah-langkah menjalankan program PHP :
1.Membuka aplikasi XAMPP Control Panel.
2.Menekan tombol Start pada bagian Apache.
3.Memastikan Apache sudah berjalan dan berwarna hijau.
4.Membuka aplikasi Visual Studio Code.
5.Membuka folder proyek lab7_php yang berada di dalam folder htdocs.
6.Membuat file PHP dan memasukkan kode program sesuai latihan.
7.Menyimpan kode menggunakan tombol Ctrl + S.
8.Membuka Google Chrome.

Mengetik alamat berikut pada browser  :
http://localhost/lab7_php/

Menekan Enter untuk melihat hasil program.

4. Struktur File
Struktur folder praktikum PHP yang digunakan adalah :

lab7_php/
 - index.php
 - README.md

Keterangan :

index.php: Berisi program dasar PHP, menampilkan waktu server, menghitung nilai akhir, menampilkan predikat, daftar mahasiswa, serta function kelulusan, formulir pencarian menggunakan metode GET, latihan pengiriman data menggunakan POST, perhitungan subtotal barang, dan Mini Project formulir data mahasiswa.

README.md: Berisi dokumentasi praktikum yang menjelaskan tujuan, perangkat, cara menjalankan server, struktur file, dan ringkasan hasil.

Hasil Praktikum

<img width="956" height="559" alt="Screenshot 2026-11-14 234123" src="https://github.com/user-attachments/assets/e26c4c42-5cd5-4d1d-b3f8-45ac8041b0ec" />

Dibuat halaman PHP sederhana menggunakan perintah echo untuk menampilkan tulisan dan waktu server.
Fungsi date() digunakan untuk menampilkan tanggal dan waktu berdasarkan server.
Hasilnya, browser berhasil menampilkan tulisan "PHP berhasil dijalankan" beserta waktu server.

<img width="959" height="563" alt="Screenshot 2026-11-14 234640" src="https://github.com/user-attachments/assets/8a37ea70-36a7-4a19-9f0e-cd58226c1762" />

Program menggunakan percabangan if, elseif, dan else untuk menentukan predikat berdasarkan nilai akhir.
Pada latihan ini dibuat program untuk menghitung nilai akhir mahasiswa berdasarkan nilai tugas, UTS, dan UAS.
Bobot penilaian yang digunakan :
Tugas: 30%
UTS: 30%
UAS: 40%

<img width="959" height="560" alt="Screenshot 2026-11-14 234756" src="https://github.com/user-attachments/assets/a70df2ca-a433-4593-a6df-35caf8e2b2a4" />
(Hasil seperti gambar diatas)

<img width="958" height="556" alt="Screenshot 2026-11-14 235147" src="https://github.com/user-attachments/assets/0564d896-de68-4b01-a819-71dc3ad50b7b" />

Pada latihan ini digunakan array untuk menyimpan beberapa nama mahasiswa.
Kemudian, perulangan foreach digunakan untuk menampilkan seluruh nama mahasiswa dalam bentuk daftar bernomor.
Maka hasil seperti berikut.
Nama mahasiswa yang ditampilkan adalah Alya, Bima, Citra, Doni, Kim, Lee, dan Park.

<img width="959" height="563" alt="Screenshot 2026-11-15 001837" src="https://github.com/user-attachments/assets/e7740ad1-048b-46a2-bb7e-5b248e26718c" /> 

Pada latihan ini dibuat function bernama cekKelulusan() untuk menentukan status kelulusan berdasarkan nilai mahasiswa.
Jika nilai mencapai 75 atau lebih, program menampilkan keterangan LULUS.
Jika nilai kurang dari 75, program menampilkan keterangan TIDAK LULUS.
Contoh pengujian menggunakan nilai 85 menghasilkan keterangan LULUS.

<img width="959" height="564" alt="Screenshot 2026-11-15 001933" src="https://github.com/user-attachments/assets/2d5be044-f433-4fa4-821b-85ca4db50a76" />

Pada latihan ini dibuat formulir pencarian menggunakan metode GET.
Pengguna dapat memasukkan kata kunci, kemudian menekan tombol Cari.

<img width="959" height="561" alt="Screenshot 2026-11-15 002216" src="https://github.com/user-attachments/assets/855caf24-adf7-4040-a6e6-11ccf94edce3" />

Data akan dikirim melalui URL browser dan ditampilkan kembali menggunakan htmlspecialchars().

<img width="957" height="563" alt="Screenshot 2026-11-15 002740" src="https://github.com/user-attachments/assets/3579723c-b62a-4b4d-abc9-8a376f1cf010" />

Pada latihan ini dibuat formulir sederhana yang berisi nama dan program studi.
Data dikirim menggunakan metode POST.
Setelah tombol Kirim Data ditekan, program akan memeriksa apakah semua kolom sudah diisi.
Jika data benar, program menampilkan nama dan program studi yang dimasukkan.

<img width="959" height="562" alt="Screenshot 2026-11-15 003205" src="https://github.com/user-attachments/assets/8d72ee70-fbe3-48c1-8a14-b2ab68266e99" />

Pada latihan ini dibuat formulir untuk menghitung subtotal harga barang berdasarkan nama barang, harga, dan jumlah pembelian.
Program melakukan validasi untuk memastikan nama barang sudah diisi, harga berupa angka, dan jumlah berupa bilangan bulat minimal 1.
Jika data benar, program menghitung subtotal dengan mengalikan harga dan jumlah barang.

<img width="959" height="539" alt="Screenshot 2026-11-15 181021" src="https://github.com/user-attachments/assets/5ba9436a-5d59-4259-b7e9-6eeed1f919e7" />

Hasil perhitungan ditampilkan dalam format rupiah.

<img width="959" height="174" alt="Screenshot 2026-11-15 181136" src="https://github.com/user-attachments/assets/dbaaa077-9195-4db7-b0b5-0384527ce3a7" />

Pada mini project ini dibuat aplikasi formulir data mahasiswa menggunakan metode POST.

<img width="958" height="227" alt="Screenshot 2026-11-15 181414" src="https://github.com/user-attachments/assets/ef6215c9-42c7-4282-af9c-7ef991d689d8" />

Program dilengkapi validasi server-side untuk memastikan seluruh data sudah sesuai.
Validasi yang digunakan meliputi :
Nama wajib diisi.
NIM wajib diisi.
Program studi wajib dipilih.
Email harus memiliki format yang valid.
Semester harus berupa bilangan bulat dari 1 sampai 14.
Jika terdapat kesalahan, program akan menampilkan seluruh pesan kesalahan.
Jika semua data valid, program akan menampilkan ringkasan data mahasiswa.
Fungsi htmlspecialchars() digunakan untuk mengamankan data sebelum ditampilkan pada halaman browser.

Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat disimpulkan bahwa PHP merupakan bahasa pemrograman server-side yang dapat digunakan untuk membuat website dinamis.
