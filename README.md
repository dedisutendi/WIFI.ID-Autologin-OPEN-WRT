# Autologin
Autologin WMS, WIFI ID, dll with OpenWRT

===============================
Script Autologin 
===============================

Instalasi
=========
1. Merk Router bebas
2. Router sudah terinstall OS OpenWRT
3. Sambungkan dengan Internet, akan ada update dan download library
4. Copy file autologin ke ROOT, (biasanya saya pakai WinSCP)
5. Gunakan PUTTY dan lakukan remote SSH Router anda
6. Jalankan perintah pada PUTTY dan tunggu sampai proses selesai :

	sh autologin

7. Untuk buka GUI ketik pada browser anda:

	http://IP-ROUTER-ANDA/cgi-bin/register

	contoh = http://192.168.1.1/cgi-bin/register

8. Isi Kolom dalam GUI, sesuaikan dengan kondisi URL Landing Page anda dan kode Voucher anda.
9. Klik SUBMIT
10. Sambungkan Router anda ke jaringan Wifi ID, WMS Venue atau Wico 2.0 anda
11. Restart
12. Selesai

Pemecahan masalah
=================
A. Jika setelah proses Instalasi dan tidak mau tersambung dengan jaringan
   1. Periksa jaringan anda
   2. Periksa apakah Jenis Voucher, Produk dan Type jaringan anda sudah sesuai (WMS Venue, WIFI ID atau WICO)
   3. Periksa di Gui apakah sudah benar data yang anda masukkan
   4. Periksa penulisan Username dan Password Voucher anda
   5. Periksa INTERFACE yang terkoneksi apakah sudah betul
   6. Jika sudah benar semua, SSH Router anda dengan PUTTY lalu jalankan perintah :

      sh auto_login

   7. Lihat proses yg berjalan dan bandingkan Informasi yg ada dengan GUI yg sudah anda input.
	
B. Jika masih belum tersambung, kemungkinan pemblokiran MAC ADDRESS Router oleh ISP Anda.
   1. Isi Kolom NEW MAC pada tampilan GUI dengan MAC ADDRESS 
      - Format penulisan : xx:xx:xx:xx:xx:xx
      - atau tulis "random" ==> huruf kecil semua dan tanpa tanda petik
   2. Klik SUBMIT
   3. Tunggu 1 menit atau lakukan SSH Router anda dengan PUTTY lalu jalankan perintah :
      
       sh auto_login

    4. Lihat hasil


===============================
Script Autologin
===============================
