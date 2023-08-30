- # __Ping__
#### Ping adalah sebuah perintah yang digunakan dalam jaringan komputer untuk mengukur waktu yang diperlukan bagi data (biasanya dalam bentuk paket) untuk pergi dari satu titik ke titik lain dalam jaringan dan kembali lagi. Pengukuran ini biasanya dilakukan dengan mengirimkan paket data ke tujuan yang ditentukan dan kemudian menerima balasan dari tujuan tersebut. Waktu yang diperlukan untuk melakukan perjalanan ini disebut sebagai "ping time" atau "round-trip time," dan sering diukur dalam milisecond (ms). Semakin rendah nilai ping time, semakin cepat koneksi dan respons jaringan.
#
# _-Contoh Penggunaan_
![ping](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/Screenshot%202023-08-28%20122705.png)
#
1. Mengirim Paket: 
Ketika menjalankan perintah ping ke sebuah alamat IP atau nama domain, sistem operasi akan membuat paket data ICMP (Internet Control Message Protocol) dengan menggunakan perintah ICMP Echo Request. Paket ini berisi permintaan untuk host tujuan merespons.

2. Mengirim ke Host Tujuan: 
Paket ICMP tersebut dikirim melalui jaringan menuju host tujuan. Setiap perangkat jaringan di antara pengirim dan penerima akan memproses paket ini sesuai dengan aturan jaringan.

3. Respon Dari Host Tujuan: 
Jika host tujuan aktif dan dapat dijangkau, ia akan merespons dengan paket balasan ICMP Echo Reply. Paket balasan ini berisi informasi bahwa host tujuan menerima paket yang dikirimkan sebelumnya.

4. Waktu Tempuh: 
Setelah paket balasan ICMP Echo Reply diterima oleh pengirim, sistem akan mencatat waktu ketika paket dikirim dan waktu ketika balasannya diterima. Selisih waktu ini memberikan informasi tentang berapa lama dibutuhkan paket untuk pergi ke tujuan dan kembali lagi. Waktu ini biasanya disebut sebagai "ping time" atau "round-trip time".

5. Statistik: 
Setelah serangkaian paket telah dikirim dan diterima, perintah ping akan memberikan statistik tentang rata-rata waktu tempuh (round-trip time), deviasi standar, dan persentase paket yang hilang (jika ada) dalam bentuk tanggapan kepada pengguna.

Perintah ping sangat berguna dalam menguji koneksi jaringan, mengevaluasi latensi, dan mendeteksi masalah konektivitas. Namun, penting untuk diingat bahwa beberapa host atau router dapat mengabaikan atau memblokir permintaan ping sebagai bagian dari kebijakan keamanan mereka
#
- # __Traceroute__
#### Traceroute adalah sebuah perintah atau alat di jaringan komputer yang digunakan untuk melacak jalur yang dilalui oleh paket data saat melakukan perjalanan dari satu titik ke titik lain dalam jaringan. Tujuan utama traceroute adalah untuk menampilkan daftar titik lompatan (hops) yang dilalui oleh paket data, serta mengukur berapa lama waktu yang dibutuhkan oleh paket data untuk mencapai setiap titik lompatan.
#
# _-Contoh Penggunaan_
![ping](https://github.com/qiau/Konsep-Jaringan/blob/main/assets/Web%20capture_28-8-2023_122559_ping.eu.jpeg)
#### Proses traceroute bekerja dengan mengirimkan serangkaian paket data ke tujuan yang ditentukan dengan mengatur nilai Time-to-Live (TTL) pada setiap paket. TTL adalah batasan jumlah lompatan (hops) yang diizinkan oleh paket sebelum dihapus dari jaringan. Setiap kali paket melewati satu lompatan, TTL akan dikurangi. Ketika TTL mencapai nol, perangkat di lompatan tersebut menghapus paket dan mengirimkan pesan balasan (icmp time exceeded) kepada pengirim.

#### Dengan cara ini, traceroute dapat mengidentifikasi setiap titik lompatan yang dilalui oleh paket data dan mengukur waktu yang dibutuhkan untuk setiap lompatan. Hasil traceroute biasanya ditampilkan dalam bentuk daftar, menunjukkan alamat IP dan waktu yang diperlukan untuk setiap titik lompatan.
