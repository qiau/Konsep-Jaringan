![apa itu Telnet](https://4.bp.blogspot.com/-N0q7e9-ZPQ0/WrHjJrXEs1I/AAAAAAAAADQ/DIr6Vnnqn4kpMw0JHGVaIP1wo7H0OWeWACLcBGAs/s1600/telnet.png)
- # _Pengertian Telnet_
#### Telnet adalah sebuah protokol jaringan yang digunakan untuk mengakses dan mengendalikan perangkat jarak jauh melalui jaringan komputer. Protokol ini memungkinkan pengguna untuk melakukan akses jarak jauh ke perangkat seperti server, router, atau komputer lainnya, seolah-olah mereka sedang duduk di depan perangkat tersebut secara fisik. Telnet menggunakan koneksi TCP/IP (Transmission Control Protocol/Internet Protocol) untuk mentransmisikan data antara komputer pengguna (client) dan komputer tujuan (server) melalui jaringan.

- # _RFC_
#### RFC (Request for Comments) adalah serangkaian dokumen yang digunakan untuk menggambarkan protokol dan standar di internet. Telnet awalnya dijelaskan dalam RFC 854, yang kemudian diperbarui oleh RFC 855, RFC 856, dan RFC 857. RFC terbaru yang terkait dengan Telnet adalah RFC 854, yang diterbitkan pada tahun 1983. Namun, penggunaan Telnet telah menurun seiring waktu karena kurangnya keamanan, dan protokol pengganti yang lebih aman seperti SSH telah menjadi lebih populer.

- # _Flowgraph_
#### Telnet adalah protokol jaringan yang berbasis TCP (Transmission Control Protocol), sehingga alur atau "flow" dari koneksi Telnet mengikuti model dasar yang sama dengan alur koneksi TCP pada umumnya.
![Telnet flowgraph](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/telnetflowgraph.png)
##### 1. Pengguna memulai koneksi Telnet dengan mengirimkan permintaan koneksi (SYN) ke server Telnet.
##### 2. Klien Telnet mengirimkan data ke server, seperti permintaan autentikasi (nama pengguna dan kata sandi).
##### 3. Server Telnet menerima data dan memprosesnya, kemungkinan dengan meminta pengguna untuk memasukkan informasi autentikasi.
##### 4. Server Telnet membalas dengan mengirimkan data balasan.
##### 5. Klien Telnet menerima data balasan dari server.
##### 6. Klien Telnet mengirimkan lebih banyak data atau perintah ke server (interaksi berlanjut).
##### 7. Server Telnet menerima perintah dari klien dan merespons dengan mengirimkan data lebih lanjut.
##### 8. Pengguna mengirimkan permintaan untuk menutup koneksi (FIN) ke server setelah selesai.
##### 9. Server Telnet merespons dengan mengirimkan konfirmasi penutupan koneksi (FIN), dan koneksi ditutup.
