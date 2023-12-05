    Nama		        : Raihan Eka Pramudya
    NRP		        : 3122600011
    Kelas		        : 2 D4 Teknik Informatika A
    Mata Kuliah	        : Konsep Jaringan
    Dosen Pengampu	        : Dr. Ferry Astika Saputra S.T., M.Sc
    
# -Arsitektur Jaringan Komputer
> Merupakan konfigurasi jaringan yang mencakup perangkat keras, perangkat lunak, protokol komunikasi, aturan, dan standar yang digunakan untuk mengatur interaksi antara perangkat dalam jaringan komputer.

# -Arsitektur yang Umum Dipakai di Kampus

Kampus atau universitas biasanya menggunakan arsitektur jaringan *Campus Area Network (CAN)* dikarenakan cakupan jaringannya lebih luas dibandingkan *Local Area Network (LAN)* karena kampus atau universitas memiliki beberapa gedung-gedung dalam lokasi yang berbeda, namun dapat terhubung dalam jaringan yang sama.

**<h4 class ="isi" style="font-family:bahnschrift;">Keuntungan lain menggunakan CAN dibandingkan LAN antara lain : </h4>**

- Dapat membagi sumber daya, seperti data, hardware, dan aplikasi di seluruh lokasi yang terhubung. Hal ini memudahkan akses sumber daya ini dari berbagai bagian kampus tanpa memerlukan infrastruktur jaringan yang terpisah di setiap lokasi.
- Kolaborasi antara Lokasi yang berbeda, dimana CAN dapat memfasilitasi kolaborasi dan komunikasi antara staf dan mahasiswa yang berada di lokasi yang berbeda, sehingga meningkatkan efisiensi kerja dan pertukaran informasi.
- Peningkatan kinerja jaringan, dengan menggunakan CAN memungkinkan transfer data yang cepat dan akses yang lebih lancar ke sumber daya jaringan.
- Pemantauan dan manajemen sentral dimana kampus dapat melakukan pemantauan dan manajemen jaringan secara sentral dari satu lokasi, sehingga dapat memudahkan pengelolaan dan pemeliharaan jaringan yang lebih efisien.
- CAN dirancang untuk dapat diperluas dan diubah sesuai dengan pertumbuhan kampus. Dengan mempertimbangkan skala dan kebutuhan yang berbeda, CAN dapat disesuaikan untuk memenuhi tuntutan infrastruktur jaringan yang terus berkembang

<h4 class ="isi" style="font-family:bahnschrift;">Contoh penggunaan Campus Area Network dengan Medium campus network architecture</h4>

<img src="assets/campus network.png"><br>

<h5 class ="isi" style="font-family:bahnschrift;">Penjelasan tiap bagian</h5>

1. Egress Layer 
    Lapisan yang menghubungkan jaringan kampus ke internet, yang biasanya membuat firewall untuk mengontrol lalu-lintas dari intranet hingga internet, serta mencegah serangan hacker yang ada pada internet yang berusaha menyerang intranet. Selain itu, Layer ini juga men-translate network address.
2. Core Layer
    Lapisan yang menghubungkan semua bagian dari jaringan kampus. Core layer biasanya terdiri dari router yang menangani lalu lintas internet yang masuk dan keluar dari jaringan kampus
3. Aggregation Layer
    Lapisan yang menghubungkan lapisan akses ke lapisan core. Aggregation layer biasanya terdiri dari router yang menangani lalu lintas internet yang masuk dan keluar dari jaringan kampus
4. Access Layer
    Lapisan yang menghubungkan komputer-komputer di dalam kampus ke jaringan. Access layer biasanya terdiri dari switch yang menghubungkan komputer-komputer di dalam kampus ke jaringan

<h5 class ="isi" style="font-family:bahnschrift;">Selain keempat layer tersebut, terdapat pula :</h5>

1. Data Center Area
    Tempat di mana komputer-komputer yang menjalankan layanan jaringan kampus berada. Data center area biasanya terletak di lokasi yang aman dan memiliki fasilitas yang memadai untuk mendukung operasi komputer.
2. AC (Access Controller)
    Perangkat jaringan yang mengelola satu atau lebih AP. AC bertanggung jawab untuk mengatur keamanan, kebijakan, dan QoS (Quality of Service) pada jaringan nirkabel.
3. AP (Access Point)
   Perangkat jaringan yang berfungsi untuk menghubungkan perangkat-perangkat wireless ke network.

Pada Medium campus network architecture, jumlah dari end user biasanya sekitar 200 hingga 2000, dan jumlah dari perangkat network biasanya sekitar 25 hingga 100 perangkat yang mana dapat mendukung beberapa ratus atau ribu pengguna menuju access.
