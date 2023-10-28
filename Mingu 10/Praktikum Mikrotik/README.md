**<h1 style="font-family:bahnschrift;">~ PENDAHULUAN</h1>**

***<h2 style="font-family:bahnschrift;">1. Mikrotik</h2>***

***<h4 style="font-family:bahnschrift;">1.1.Pengertian Mikrotik</h4>***
> <div class ="isi" style="font-family:bahnschrift;"> Mirkrotik ialah sistem operasi yang berbasis perangkat lunak (software) yang dipergunakan untuk menjadikan komputer sebagai router sebuah jaringan. Mikrotik juga menggunakan sistem operasi berbasis Linux dan menjadi dasar network router. Sistem operasi (OS) ini sangat cocok untuk membangun administrasi jaringan komputer yang berskala kecil hingga besar.
> 
***<h4 style="font-family:bahnschrift;">1.2.Fungsi Mikrotik</h4>*** 

- <div class ="isi" style="font-family:bahnschrift;"> Memberikan sistem otentikasi
- <div class ="isi" style="font-family:bahnschrift;"> Konfigurasi jaringan lokal
- <div class ="isi" style="font-family:bahnschrift;"> Mengelola sistem jaringan internet
- <div class ="isi" style="font-family:bahnschrift;"> Memberikan peran sebagai hotspot
- <div class ="isi" style="font-family:bahnschrift;"> Membuat PPPoE Server

***<h4 style="font-family:bahnschrift;">1.3. Jenis Mikrotik</h4>*** 

- <div class ="isi" style="font-family:bahnschrift;"> Mikrotik RouterOS  
  
    > Sistem operasi yang dipakai berbasis UNIX yang menyediakan fitur mulai dari paket router, bridge, firewall, proxy server, hotspot dan lain sebagainya. Dengan Mikrotik ini memungkinkan untuk membangun router sendiri hanya dengan menggunakan sebuah OS. 
    
- <div class ="isi" style="font-family:bahnschrift;"> RouterBoard
    
  >RouterBoard berukuran sangat kecil dan lebih praktis, yang dapat melakukan proses instalasi RouterOS pada RouterBoard yang telah terkonfigurasi dengan baik. RouterBoard terdiri dari sebuah processor, ROM, RAM, dan flash memory.

***<h4 style="font-family:bahnschrift;">1.4. Manfaat Mikrotik</h4>*** 

- <div class ="isi" style="font-family:bahnschrift;"> Sebagai <i>Internet Gateway</i> pada jaringan lokal
- <div class ="isi" style="font-family:bahnschrift;"> Sebagai penghubung antar jaringan, atau routing
- <div class ="isi" style="font-family:bahnschrift;"> Sebagai <i>Access point</i>

**<h1 style="font-family:bahnschrift;">~ PERCOBAAN</h1>**
- ### _1. WinBox_

#### 1. Mengisi Address pada Address List
<img src="assets/addAddress.png"> <br>
- #### - Isi address untuk router sesuai nomor kelompok
<img src="assets/addAddress1.png"> <br>
##### Kelompok 7 maka address kita isi dengan 10.252.108.17/24, network (10.252.108.0), dan interface ether1.
- #### - Isi IP address untuk tiap PC kelompok 7
<img src="assets/addAddress2.png"> <br>
##### Address kita isi dengan 192.168.7.1/24, network (192.168.7.0), dan interface bridge1.
- #### - Tampilan setelah terisi
<img src="assets/addAddress3.png"> <br>

#### 2. Mengisi Route pada Route List
<img src="assets/addRoute.png"> <br>
- #### - Tambahkan Route baru 
<img src="assets/AddRoute2.png"> <br>
##### Dst. Address kita isi dengan 192.168.1.0 dengan Gateway 10.252.108.11.
- #### - Tambahkan route untuk semua kelompok (1-10)
<img src="assets/AddRoute3.png"> <br>
##### Lakukan cara yang sama untuk menambahkan route baru setiap kelompok.

#### 3. Menambahkan Bridge & Ports
<img src="assets/bukabridge.jpg"> <br>
- #### - Tambahkan interface
<img src="assets/bridge1.png"> <br>
##### Isi Name dengan bridge1.
- #### - Tambahkan Ports (untuk tiap kelompok)
<img src="assets/ether.png"> <br>
<img src="assets/ether2.png"> <br>

#### 4. Menambahkan DHCP Server
<img src="assets/DHCP1.png"> <br>
<img src="assets/DHCP2.png"> <br>
<img src="assets/DHCP3.png"> <br>
<img src="assets/DHCP4.png"> <br>
<img src="assets/DHCP5.png"> <br>
<img src="assets/DHCP6.png"> <br>
<img src="assets/DCHP7.png"> <br>

#### 5. Melakukan PING antar kelompok
- #### - Percobaan terhadap kelompok 1
<img src="assets/Ping1.png"> <br>
##### Isi Name dengan bridge1.
- #### - Percobaan terhadap kelompok 2
<img src="assets/Ping2.png"> <br>

#### Proses ping dengan kelompok 1 dan 2 berhasil, hal yang sama dapat kita lakukan dengan kelompok lain (kelompok 3-10).
#
- ### _2. Topologi dalam Cisco Packet Tracer_
<img src="assets/topologi10.jpeg"> <br>

#### 1. Konfigurasi PC
- #### - Mengatur Default Gateway pada tiap PC sesuai kelompok
#### Kelompok 7
<img src="assets/PC_kel7.png"> <br>
#### Kelompok 8
<img src="assets/PC_kel8.png"> <br>
- #### - Mengisi IP address pada tiap PC sesuai kelompok
#### Kelompok 7
<img src="assets/PC_kel7.1.png"> <br>
<img src="assets/PC_kel7.2.png"> <br>
<img src="assets/PC_kel7.3.png"> <br>
#### Kelompok 8
<img src="assets/PC_kel8.1.png"> <br>
<img src="assets/PC_kel8.2.png"> <br>
<img src="assets/PC_kel8.3.png"> <br>

#### 2. Konfigurasi sub-Router
- #### - Mengatur IP dan Subnet pada FastEthernet yang terhubung ke tiap PC (3 pc)
#### Kelompok 7
<img src="assets/IP_kel7.1.png"> <br>
#### Kelompok 8
<img src="assets/IP_kel8.1.png"> <br>
- #### - Mengatur IP dan Subnet pada FastEthernet yang terhubung ke Router Utama
#### Kelompok 7
<img src="assets/IP_kel7.2.png"> <br>
<img src="assets/IP_kel7.3.png"> <br>
#### Kelompok 8
<img src="assets/IP_kel8.2.png"> <br>
<img src="assets/IP_kel8.3.png"> <br>

### Demikian Laporan Percobaan dari kelompok 7, dengan menggunakan winbox dan juga Cisco Packet Tracer
