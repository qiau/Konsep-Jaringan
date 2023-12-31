- # _Pengertian OSI_
##### OSI (Open Systems Interconnection) adalah sebuah model referensi yang diciptakan oleh International Organization for Standardization (ISO) sebagai pedoman untuk merancang dan memahami arsitektur komunikasi dalam jaringan komputer. Tujuan utama dari model OSI adalah untuk menguraikan proses komunikasi menjadi tujuh lapisan yang berbeda, masing-masing memiliki tugas spesifik dalam mengatur interaksi antara perangkat dalam jaringan.

![N|Solid](https://3.bp.blogspot.com/-eAoFvRFoeKs/W4-VrhLoXBI/AAAAAAAAC_s/2Nn6JQJ2HrkqefHrAsRlLJlcxGvblknZgCLcBGAs/s1600/7-layer-osi%25281%2529.png)

### 1. Physical Layer:
Lapisan ini berurusan dengan transmisi bit mentah melalui media fisik seperti kabel tembaga, serat optik, atau gelombang radio. Tugas utamanya adalah menangani aspek fisik dari transmisi data, termasuk sinyal, tegangan, kecepatan, dan penghubung fisik.

### 2. Data Link Layer:
Lapisan ini bertanggung jawab untuk mengelola koneksi langsung antara dua perangkat di jaringan. Fungsi utamanya termasuk pengenal pengiriman (MAC addressing), deteksi dan koreksi kesalahan (error detection and correction), serta mengatur akses media untuk mencegah tabrakan data.

### 3. Network Layer:
Lapisan ini mengatur pengiriman paket data dari sumber ke tujuan melalui berbagai jaringan dan perangkat perantara. Ini melibatkan routing, pengalamatan logis (IP addressing), fragmentasi, dan pengiriman paket melalui jaringan yang berbeda.

### 4. Transport Layer:
Lapisan ini menyediakan layanan pengiriman data end-to-end yang dapat diandalkan dan terjamin. Ini termasuk segmentasi data, pengaturan aliran (flow control), pengontrolan kesalahan, dan pengaturan koneksi seperti TCP (Transmission Control Protocol).

### 5. Session Layer:
Lapisan ini mengelola, mempertahankan, dan mengendalikan sesi komunikasi antara dua perangkat. Ini termasuk pembuatan, pemeliharaan, dan penghentian sesi. Lapisan sesi juga dapat mengontrol sinkronisasi dan manajemen dialog antara aplikasi di kedua ujung.

### 6. Presentation Layer:
Lapisan ini menangani konversi dan manipulasi data agar dapat dipahami oleh penerima. Ini meliputi enkripsi, kompresi, konversi format data, dan penanganan representasi data yang berbeda antara perangkat yang berbeda.

### 7. Application Layer:
Lapisan ini adalah lapisan tertinggi dan berisi aplikasi dan layanan yang digunakan oleh pengguna akhir. Ini adalah lapisan tempat interaksi langsung dengan pengguna terjadi. Beberapa protokol yang terkait dengan lapisan ini meliputi HTTP (Hypertext Transfer Protocol), SMTP (Simple Mail Transfer Protocol), dan FTP (File Transfer Protocol)
# 
#
#
#
![N|Solid](https://www.nesabamedia.com/wp-content/uploads/2017/10/OSI-WORKS-2.png)

- # _Mengirim Data_

| Layer | Cara Kerja |
| ------ | ------ |
| Application | Proses dimulai di lapisan aplikasi, di mana aplikasi pengirim menghasilkan data yang akan dikirimkan, seperti pesan email atau permintaan halaman web. |
| Presentation | Data dari aplikasi dapat mengalami konversi format di lapisan presentasi, seperti enkripsi data untuk keamanan atau kompresi data untuk efisiensi. |
| Session | Lapisan sesi memulai, memelihara, dan mengakhiri sesi komunikasi antara aplikasi pengirim dan penerima. Ini melibatkan pembentukan dialog dan manajemen aliran data. |
| Transport | Data dari lapisan sesi dipecah menjadi segmen atau paket yang lebih kecil di lapisan transport. Lapisan ini juga menambahkan informasi pengelolaan aliran data dan nomor urut untuk memastikan pengiriman yang andal. |
| Network | Segmen atau paket dari lapisan transport diteruskan ke lapisan jaringan, di mana alamat tujuan ditambahkan. Protokol di lapisan jaringan (misalnya, IP) mengatur pengiriman paket melalui rute yang tepat ke tujuan. |
| Data Link | Di lapisan ini, paket dari lapisan jaringan dikemas dalam frame dengan tambahan informasi seperti alamat MAC (Media Access Control). Lapisan ini mengelola akses ke media transmisi dan mendeteksi serta mengoreksi kesalahan pada level frame. |
| Physical | Frame dari lapisan link data diubah menjadi sinyal fisik yang sesuai dengan media transmisi yang digunakan, seperti sinyal listrik pada kabel atau gelombang radio. |

- # _Menerima Data_

| Layer | Cara Kerja |
| ------ | ------ |
| Physical | Pada penerima, sinyal fisik diubah kembali menjadi frame pada lapisan data link. |
| Data Link | Frame diteruskan ke lapisan link data, di mana frame diurai dan diperiksa untuk kesalahan. Jika ada kesalahan, frame dapat diperbaiki atau diabaikan. |
| Network | Data dari frame di lapisan link data dipecah dari frame dan alamat tujuan diidentifikasi. Data kemudian diteruskan ke lapisan jaringan. |
| Transport | Data di lapisan transport dikembalikan ke bentuk aslinya dari segmen atau paket, dan informasi pengelolaan aliran serta nomor urut dikelola. |
| Session | Lapisan sesi mengelola pembentukan, pemeliharaan, dan pengakhiran sesi komunikasi antara aplikasi pengirim dan penerima. |
| Presentation | Data di lapisan presentasi didekripsi atau dikompresi sesuai kebutuhan.|
| Application | Data yang telah diolah dan didekode sampai ke bentuk asli dikirimkan ke aplikasi penerima, yang kemudian dapat mengambil tindakan yang sesuai berdasarkan data tersebut. |

