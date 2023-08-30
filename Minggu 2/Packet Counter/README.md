- # __Analisis Flow Graph__
#### Packet Counter adalah perangkat yang membantu menghitung dan memvisualisasikan paket atau frame dalam sesi pemantauan atau capture. perangkat ini memberikan informasi krusial seperti jumlah total paket untuk mengukur aktivitas jaringan, laju masuk paket untuk mengidentifikasi puncak aktivitas, distribusi paket untuk memahami pola sebaran, burst rate untuk mengidentifikasi lonjakan tiba-tiba, dan waktu awal burst untuk konteks aktivitas. Dengan fungsi-fungsinya ini, Packet Counter menjadi alat analitis yang membantu pengguna memahami dinamika dan mengambil tindakan yang diperlukan untuk menjaga performa dan stabilitas jaringan.
#
![Packet Counter](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/packetcounter.png)
#
- #### Dari capture Packet Counter di atas, dapat disimpulkan bahwa ada 4 paket HTTP yang direkam, semuanya terkait dengan lalu lintas HTTP. 
- #### Dari 4 paket ini, 2 adalah permintaan (request) HTTP yang semuanya menggunakan metode GET. Sisanya adalah respon dari server web, dengan semua respon memiliki kode status HTTP dalam kategori 2xx (keberhasilan), khususnya "200 OK". 
- #### Burst rate untuk baik permintaan GET maupun respon adalah 0.0100 paket per detik, dengan burst rate pertama kali dimulai pada saat yang berbeda (0.911 detik untuk permintaan GET dan 3.956 detik untuk respon). 
- #### Laju masuk rata-rata adalah 0.0005 paket per milidetik. Jadi, capture ini menunjukkan bahwa terdapat pertukaran data HTTP yang terutama terdiri dari permintaan GET dan respon 200 OK yang berhasil.
