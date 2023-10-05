![soal cisco](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/tugas.jpeg)
- # _CISCO PACKET TRACER_
##### Sebuah topologi jaringan yang telah dirancang dan dikonfigurasi dalam lingkungan simulasi menggunakan Cisco Packet Tracer. Topologi jaringan adalah susunan fisik dan logis dari perangkat jaringan yang terinterkoneksi, yang berfungsi sebagai kerangka kerja untuk pertukaran data dan sumber daya di dalam jaringan. Dalam konteks ini, kita akan menjelajahi implementasi konkret dari topologi yang melibatkan dua router, dua switch, dan empat komputer (PC).
##### Untuk menjalankan agar jaringan berfungsi, kita perlu mengonfigurasi router dan pc dengan benar. Berikut adalah langkah-langkahnya:

#### 1. Membuat kerangka desain dengan menambahkan router (model router 1841), tambahkan switch (model switch 2950-24), dan tambahkan End Device menggunakan (model PC). 
#### Hasilnya akan seperti gambar berikut.
![pt 1](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.1.png)
#
#### 2. Mengubah config dari Router0 (ubah IP address FastEthernet0/0 dan FastEthernet0/1) serta menambahkan RIP routing.
#### Berturut-turut hasilnya akan seperti gambar berikut.
![pt 2](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.2.png)
![pt 3](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.3.png)
![pt 4](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.4.png)
#
#### 3. Mengubah config dari Router1 (ubah IP address FastEthernet0/0 dan FastEthernet0/1) serta menambahkan RIP routing.
#### Berturut-turut hasilnya akan seperti gambar berikut.
![pt 5](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.5.png)
![pt 6](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.6.png)
![pt 7](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.7.png)
#
#### 4. Mengubah config dari PC0 (menambahkan IPv4 address, subnet mask, dan default gateway).
#### Hasilnya akan seperti gambar berikut.
![pt 8](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.8.png)
#
#### 5. Mengubah config dari PC1 (menambahkan IPv4 address, subnet mask, dan default gateway).
#### Hasilnya akan seperti gambar berikut.
![pt 9](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.9.png)
#
#### 6. Mengubah config dari PC2 (menambahkan IPv4 address, subnet mask, dan default gateway).
#### Hasilnya akan seperti gambar berikut.
![pt 10](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.10.png)
#
#### 7. Mengubah config dari PC3 (menambahkan IPv4 address, subnet mask, dan default gateway).
#### Hasilnya akan seperti gambar berikut.
![pt 11](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.11.png)
#
#### 8. Langkah selanjutnya menambahkan kabel koneksi antar perangkat router (dengan kabel Copper Cross-Over), koneksi router dengan Switch (dengan kabel Copper Straight-Through), dan  koneksi switch dengan perangkat PC (dengan kabel Copper Straight-Through),
#### Hasilnya akan seperti gambar berikut.
![pt 12](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.12.png)
#
#### 9. Setelah semua terhubung maka kita lakukan ping menggunakan CMD pada masing-masing PC.
- #### PC0 dengan PC1 (sesama router), PC0 dengan PC2 dan PC3 (berbeda router) berturut-turut sebagai berikut.
![pt 13](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.13.png)
#### Percobaan ping berhasil!
#
- #### PC1 dengan PC0 (sesama router), PC1 dengan PC2 dan PC3 (berbeda router) berturut-turut sebagai berikut.
![pt 14](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.14.png)
#### Percobaan ping berhasil!
#
- #### PC2 dengan PC3 (sesama router), PC2 dengan PC0 dan PC1 (berbeda router) berturut-turut sebagai berikut.
![pt 15](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.15.png)
#### Percobaan ping berhasil!
#
- #### PC3 dengan PC2 (sesama router), PC3 dengan PC0 dan PC1 (berbeda router) berturut-turut sebagai berikut.
![pt 16](https://github.com/qiau/Konsep-Jaringan/blob/main/Minggu%207/Packet%20Tracer/assets/1pt.16.png)
#### Percobaan ping berhasil!
#
## Kesimpulan
#### Perlu dipahami bahwa router adalah komponen kunci yang menghubungkan berbagai subnet di jaringan, sementara switch berperan penting dalam mengarahkan lalu lintas data antar perangkat dalam subnet yang sama. Sedangkan, komputer (PC) berfungsi sebagai entitas pengguna akhir yang memerlukan konfigurasi yang tepat untuk berkomunikasi dengan perangkat di luar subnet mereka.

