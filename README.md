# Internship-2
Pengujian Metode Stress Testing Menggunakan Metode Apache Benchmark

## Intalasi 
- Pada Ubuntu atau Debian, Apache Benchmark(ab) adalah bagian dari paket apache2-utils. Jadi pastikan paket telah terinstal untuk menjalankan fungsi apache benchmark.
- Untuk menginstall apache benchmark silahkan masukkan:


a. Ubuntu/ Debian:
apt-get install apache2-utils

b. RHEL/CentOS/Fedora:
yum install http-tools

Setelah proses instalasi atau pemasangan selesai, selanjutnya kita dapat mencoba pengetesan menggunakan apache benchmark, dengan mengeksekusi perintah ke alamat URL yang dituju. Berikut contoh pengujian menggunakan Apache Benchmark:

ab -k -c 50 -n 1000 "http://situstujuan.com"

Keterangan:
-k Mengirimkan instruksi ke web server agar koneksi yang sudah dibuka tidak ditutup melainkan digunakan ulang. Ini meniru perilaku browser.
-c Berapa banyak koneksi bersamaan yang dibuka. Bisa dianalogikan dengan banyaknya pengunjung dalam satu waktu.
-n Jumlah permintaan konten yang akan dibuat ke web server.