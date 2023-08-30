- # __Analisis http.cap, telnet-cooked.cap, dan dns.cap pada Wireshark__
### Perlu diketahui bahwa pada wireshark terdapat beberapa informasi yaitu seperti:
- ### No: yang bertujuan menampilkan urutan paket data yang direkam
- ### Time: menampilkan waktu pada saat mengakses paket ke tujuan
- ### Source: menampilkan alamat ip pengguna/pengakses
- ### Destination: menampilkan alamat ip dari tujuan data
- ### Protocol: menampilkan informasi protocol pada saat mengakses data tersebut
- ### Info: menampilkan informasi yang ditampilkan pada proses capture data tersebut
#
## 1. http.cap
![http.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/httpall.png)
#
#### Pada snapshot dari file http.cap diatas, menampilkan informasi berbagai source, Destinasi, protocol, dsb. Dapat dilihat protocol yang berlangsung pada transaksi tersebut menggunakan TCP, DNS, dan HTTP.
#### Pada no-4, yang memiliki protocol HTTP dengan informasi /download.html HTTP/1.1, dapat dilihat pada bagian frame, yang berisi informasi sebagai berikut :
![httpframe.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/httpframe.png)
#
#### Pada bagian frame, berisi informasi arrival time koneksi tersebut dilakukan, yakni pada tanggal 13 Mei 2004
#### Selain itu, terdapat informasi panjang frame yang terkirim, yakni sebesar 533 bytes, atau setara dengan 4264 bits
#### Kemudian ada informasi protocol yang digunakan dalam frame tersebut, yakni eth:ethertype:ip:tcp:https
#
## 2. telnet-cooked.cap
![telnet.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/telnetall.png)
#
#### Pada snapshot dari file telnet-cooked.cap diatas, menampilkan informasi berbagai source, Destinasi, protocol, dsb. Dapat dilihat protocol yang berlangsung pada transaksi tersebut menggunakan TCP, dan TELNET
#### Pada nomor 5, dapat dilihat detail untuk frame yang berisi informasi sebagai berikut :
![telnetframe.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/telnetframe.png)
#
#### Pada snapshot diatas, dapat dilihat beberapa informasi yang berisi arrival time, pada 28 November 1999, Jumlah frame sebanyak 5, panjang frame sepanjang 69 Bytes, atau setara dengan 552 bits.
#
## 3. dns.cap
![dns.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/dnsall.png)
#
#### Pada snapshot dari file dns.cap diatas, menampilkan informasi berbagai source, Destinasi, protocol, dsb. Dapat dilihat protocol yang berlangsung pada transaksi tersebut menggunakan DNS.
#### Pada no-4, yang mana terdapat respon dari domain tertentu dengan beberapa detail sebagai berikut :
![dnsframe.cap](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/dnsframe.png)
#### Pada snapshot diatas dapat dilihat bahwa domain yang memberikan response ialah google.com.
