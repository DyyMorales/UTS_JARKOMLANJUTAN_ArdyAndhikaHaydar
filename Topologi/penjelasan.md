# Penjelasan Topologi

## Skema IP Addressing
Setiap perangkat diberi alamat IP yang unik untuk mengidentifikasi masing-masing jaringan.
## Router di setiap Area:
o	Area 1: Router memiliki IP LAN 192.168.1.1. <br>
o	Area 2: Router memiliki IP LAN 192.168.2.1. <br>
o	Area 3: Router memiliki IP LAN 192.168.3.1. 
## Komputer di setiap Area:
o	Komputer A (Area 1): IP-nya adalah 192.168.1.2 dengan gateway 192.168.1.1. <br>
o	Komputer B (Area 2): IP-nya adalah 192.168.2.2 dengan gateway 192.168.2.1. <br>
o	Komputer C (Area 3): IP-nya adalah 192.168.3.2 dengan gateway 192.168.3.1.
## IP untuk Koneksi Antar-Router:
o	Router 1 ke Router 2: 10.0.0.1 (di Router 1) dan 10.0.0.3 (di Router 2). <br>
o	Router 1 ke Router 3: 10.0.0.2 (di Router 1) dan 10.0.0.5 (di Router 3). <br>
o	Router 2 ke Router 3: 10.0.0.4 (di Router 2) dan 10.0.0.6 (di Router 3).
## Routing dan Komunikasi
Setiap router dikonfigurasi dengan rute ke jaringan di dua area lain. Ini memastikan bahwa jika Komputer A di Area 1 ingin mengirim data ke Komputer B di Area 2, data akan dialihkan melalui router dan melewati jaringan WAN yang menghubungkan ketiga area.
## Dengan konfigurasi ini:
Komputer A, B, dan C dapat saling berkomunikasi, meskipun berada di jaringan lokal yang berbeda dan terhubung melalui router di setiap area.
