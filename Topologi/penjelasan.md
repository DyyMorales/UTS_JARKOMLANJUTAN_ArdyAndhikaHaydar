## Penjelasan komponen pada topologi tersebut:

## Internet Cloud:

terdapat cloud yang melambangkan jaringan internet. Internet digunakan sebagai media penghubung untuk menghubungkan jaringan di tiga lokasi berbeda melalui VPN Tunnel. <br>

## Router:

Setiap lokasi (KJ, CR, dan KHI) memiliki satu perangkat router. Router ini berfungsi sebagai penghubung jaringan lokal di masing-masing lokasi dengan jaringan internet. <br>

## VPN Tunnel: 
Setiap router memiliki konfigurasi VPN Tunnel untuk membuat jalur komunikasi yang aman antara lokasi-lokasi tersebut melalui internet. VPN Tunnel berfungsi sebagai saluran terenkripsi untuk melindungi data yang dikirimkan antar lokasi. <br>

## Switch:

Setelah melewati router, setiap lokasi memiliki switch yang terhubung ke router masing-masing. Switch ini berfungsi untuk menghubungkan perangkat-perangkat komputer di dalam jaringan lokal pada lokasi tersebut. <br>
Switch menerima data dari router dan mendistribusikannya ke perangkat-perangkat komputer di jaringan lokal.

## PC (Personal Computer):

Di setiap lokasi terdapat beberapa PC yang terhubung ke switch. <br>
Di lokasi KJ: terdapat tiga PC yang dinamai PC1, PC2, dan PC3. <br>
Di lokasi CR: terdapat tiga PC dengan nama PC4, PC5, dan PC6. <br>
Di lokasi KHI: terdapat tiga PC dengan nama PC7, PC8, dan PC9. <br>
PC ini dapat berkomunikasi dengan PC lain di lokasi berbeda melalui koneksi VPN Tunnel yang dibuat antara router masing-masing lokasi.

## Fungsi Setiap Lokasi:

KJ, CR, dan KHI merupakan tiga lokasi fisik yang terpisah, namun terhubung dalam satu jaringan yang saling berkomunikasi. Koneksi antar lokasi ini memanfaatkan internet sebagai media komunikasi dan menggunakan VPN Tunnel untuk keamanan data.
Topologi ini cocok untuk organisasi dengan kantor cabang yang tersebar di lokasi berbeda, yang memerlukan koneksi aman untuk mengakses data atau sistem secara terpusat. <br>
Dengan menggunakan topologi ini, semua perangkat komputer di lokasi KJ, CR, dan KHI dapat berkomunikasi secara langsung dan aman melalui VPN Tunnel yang terenkripsi, meskipun menggunakan jaringan internet sebagai penghubung utama.
