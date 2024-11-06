## Rincian IP Address dan Alur Koneksi
## 1. Cloud (Internet)
IP Address Cloud (Gateway): 192.168.0.1/24 <br>
Peran: Cloud berfungsi sebagai gateway utama untuk akses internet. Setiap router akan mengarah ke IP ini sebagai alamat gateway pada port WAN mereka.

## 2. Router dan Koneksi ke Cloud
## Router 1:

## WAN Interface:
IP: 192.168.0.2/24 (IP ini diatur sebagai WAN IP untuk terhubung ke cloud), <br>
Gateway: 192.168.0.1 (IP cloud sebagai gateway internet) <br>
LAN Interface (ke Switch 1): <br>
IP: 10.1.1.1/24 <br>
Peran: Router 1 menghubungkan jaringan lokal di Switch 1 ke cloud melalui WAN. Semua perangkat di bawah Switch 1 akan memiliki gateway 10.1.1.1. 

## Router 2:

WAN Interface: <br>
IP: 192.168.0.3/24 <br>
Gateway: 192.168.0.1 (IP cloud sebagai gateway internet) <br>
LAN Interface (ke Switch 2): <br>
IP: 10.2.2.1/24 <br>
Peran: Router 2 menghubungkan jaringan lokal di Switch 2 ke cloud. Semua perangkat di bawah Switch 2 akan menggunakan gateway 10.2.2.1. <br>

## Router 3:

WAN Interface: <br>
IP: 192.168.0.4/24 <br>
Gateway: 192.168.0.1 (IP cloud sebagai gateway internet) <br>
LAN Interface (ke Switch 3): <br>
IP: 10.3.3.1/24 <br> 
Peran: Router 3 menghubungkan jaringan lokal di Switch 3 ke cloud. Semua perangkat di bawah Switch 3 akan menggunakan gateway 10.3.3.1. <br>

## 3. Switch dan PC dalam Jaringan Lokal
Setiap switch terhubung ke router yang berbeda dan menghubungkan tiga PC dalam jaringan lokal masing-masing: <br>

Switch 1 (di bawah Router 1): <br>

PC IPs: <br>
PC1: 10.1.1.2 <br>
PC2: 10.1.1.3 <br>
PC3: 10.1.1.4 <br>
Gateway untuk semua PC: 10.1.1.1 <br>

Switch 2 (di bawah Router 2): <br>

PC IPs: <br>
PC4: 10.2.2.2 <br>
PC5: 10.2.2.3 <br>
PC6: 10.2.2.4 <br>
Gateway untuk semua PC: 10.2.2.1 <br>

Switch 3 (di bawah Router 3): <br>

PC IPs: <br>
PC7: 10.3.3.2 <br>
PC8: 10.3.3.3 <br>
PC9: 10.3.3.4 <br>
Gateway untuk semua PC: 10.3.3.1 <br>

## Alur Koneksi
Router ke Cloud: <br>

Setiap router tersambung ke cloud melalui WAN interface menggunakan IP di subnet 192.168.0.1. <br>
Cloud bertindak sebagai gateway dengan IP 192.168.0.1, dan setiap router mengarahkan lalu lintas internet ke IP ini. <br>

## Router ke Switch dan PC:

Masing-masing router terhubung ke switch melalui LAN interface dan menyediakan IP di subnet berbeda (10.1.1.1, 10.2.2.2, 10.3.3.3). <br>
Setiap PC yang terhubung ke switch menerima IP di subnet LAN masing-masing router dan menggunakan IP router sebagai gateway.
