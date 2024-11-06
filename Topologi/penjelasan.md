# Penjelasan Topologi

## Skema IP Addressing
Setiap perangkat diberi alamat IP yang unik untuk mengidentifikasi masing-masing jaringan.
## Router di setiap Area:
o	R1 KJ: Router memiliki IP LAN 192.168.1.1. <br>
o	R2 CR: Router memiliki IP LAN 192.168.2.1. <br>
o	R3 KHI: Router memiliki IP LAN 192.168.3.1. <br>
o R4 Central : bertugas menjadi WAN atau menjadi penyalur file antara PC
## Komputer di setiap Area:
o	PC1 (R1 KJ): IP-nya adalah 192.168.1.2 dengan gateway 192.168.1.1. <br>
o	PC2 (R2 CR): IP-nya adalah 192.168.2.2 dengan gateway 192.168.2.1. <br>
o	PC3 (R3 KHI): IP-nya adalah 192.168.3.2 dengan gateway 192.168.3.1.
## IP untuk Koneksi Antar-Router:
o	R1 KJ ke R2 CR: 10.0.0.1 (di R1 KJ) dan 10.0.0.3 (di R2 CR). <br>
o	R1 KJ ke R3 KHI: 10.0.0.2 (di R1 KJ) dan 10.0.0.5 (di R3 KHI). <br>
o	R2 CR ke R3 KHI: 10.0.0.4 (di R2 CR) dan 10.0.0.6 (di R3 KHI).
## Routing dan Komunikasi
Setiap router dikonfigurasi dengan rute ke jaringan di dua area lain. Ini memastikan bahwa jika PC1 di R1 KJ ingin mengirim data ke PC2 di R2 CR, data akan dialihkan melalui router dan melewati jaringan WAN yang menghubungkan ketiga area.
## Dengan konfigurasi ini:
PC 1, 2, dan 3 dapat saling berkomunikasi, meskipun berada di jaringan lokal yang berbeda dan terhubung melalui router di setiap area.
