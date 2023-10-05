Simulasi Jaringan menggunakan Cisco Packet Tracer
> Menghubungkan perangkat yang berbeda router menggunakan Cisco Packet Tracer dengan design mendesain beberapa perangkat seperti router, switch, dan PC, yang nantinya di tes koneksinya menggunakan terminal yang ada pada Cisco Packet Tracer.

Langkah-langkah
1. Membuat desain router
    Tambahkan router menggunakan model router 1841
<img src="assets/step 1.png">

2. Membuat desain switch
   Tambahkan router menggunakan model switch 2950-24
<img src="assets/step 2.png">

3. Membuat desain PC
   Tambahkan End Device menggunakan model PC
<img src="assets/step 3.png">

4. Menambahkan kabel koneksi antar perangkat router
   Tambahkan kabel antar router berupa Copper Cross-Over dengan FastEthernet 0/1
<img src="assets/step 4.png">

5. Menambahkan kabel koneksi antara router dengan Switch
   Tambahkan Copper Straight-Through dari perangkat router ke perangkat switch
   <img src="assets/step 6.png">
   <img src="assets/step 5.png">

6. Menambahkan kabel koneksi antara switch dengan perangkat PC
   Copper Straight-Through dari perangkat switch ke perangkat PC, sehingga menjadi seperti berikut :
   <img src="assets/step 7.png">

7. mengubah config dari router0 dan
   Mengubah IP address untuk FastEthernet0/1 dan FastEthernet0/0 serta menambahkan RIP routing
   <img src="assets/step 8.png">
   <img src="assets/step 9.png">
   <img src="assets/step 13.png">

8. Mengubah config dari router1 dan
   Mengubah IP address untuk FastEthernet0/1 dan FastEthernet0/0
   <img src="assets/step 10.png">
   <img src="assets/step 11.png">

9. Mengubah config dari PC0
   Menambahkan IPv4 address, dan default gateway address
   <img src="assets/step 12.png">

10. Mengubah config dari PC1
    Menambahkan IPv4 address, dan default gateway address
    <img src="assets/step 14.png">
   
11. Mengubah config dari PC2
    Menambahkan IPv4 address, dan default gateway address
    <img src="assets/step 15.png">

12. Mengubah config dari PC3
    Menambahkan IPv4 address, dan default gateway address
    <img src="assets/step 16.png">

13. Melakukan ping untuk sesama router
   Dengan membuka command prompt pada PC0
   <img src="assets/step 20.png">
   ketikkan ping 192.168.1.20
   <img src="assets/step 17.png">
      >Perintah ini digunakan untuk melakukan ping pada PC1, yang mana masih berada dalam router yang sama

14. Melakukan ping untuk router yang berbeda
   Dengan membuka command prompt pada PC0
   <img src="assets/step 20.png">
   ketikkan ping 192.168.2.10
   <img src="assets/step 18.png">
   >Perintah ini digunakan untuk melakukan ping pada PC3, yang mana berada dalam router yang berbeda
