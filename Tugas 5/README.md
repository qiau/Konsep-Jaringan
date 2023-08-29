![three-way handshake](main/assets/applsci-06-00358-g001-550.jpg)

- # __PENGERTIAN__
##### Three-way handshake adalah proses tiga langkah yang digunakan oleh protokol TCP (Transmission Control Protocol) untuk memulai koneksi antara dua perangkat dalam jaringan komputer. Tujuan dari tiga langkah ini adalah untuk memastikan bahwa pengirim dan penerima siap untuk berkomunikasi dan untuk memastikan bahwa koneksi awal berjalan dengan lancar. Tiga langkah ini melibatkan pengiriman tiga pesan secara berurutan antara pengirim dan penerima.

1. First Step (SYN):
Pengirim mengirimkan pesan SYN (synchronize) ke penerima. Ini adalah permintaan untuk memulai koneksi dan mencakup nomor urut acak sebagai "nomor urut awal". Pesan ini mengindikasikan niat pengirim untuk berkomunikasi.

2. Second Step (SYN-ACK):
Penerima menerima pesan SYN dari pengirim dan mengirimkan balasan SYN-ACK (synchronize-acknowledge) kembali. Balasan ini mencakup nomor urut acak baru sebagai "nomor urut awal" untuk penerima, dan nomor pengakuan yang sama dengan nomor urut yang diterima dari pengirim. Pesan ini menunjukkan penerimaan permintaan dan kesiapan untuk menerima data.

3. Third Step (ACK):
Pengirim menerima pesan SYN-ACK dari penerima dan mengirimkan pesan ACK (acknowledge) kembali. Pesan ini berisi nomor pengakuan yang lebih besar dari nomor urut awal yang diterima dari penerima. Pesan ini menunjukkan bahwa pengirim telah menerima balasan SYN-ACK dan siap untuk memulai pertukaran data.

Setelah langkah-langkah tersebut diselesaikan koneksi mulai terbentuk dan pengiriman data dapat dimulai.  Melalui tiga langkah ini (SYN, SYN-ACK, dan ACK), pengirim dan penerima menyelaraskan kesiapan untuk berkomunikasi, memastikan data dapat dikirim dan diterima secara andal, serta meminimalkan risiko kesalahan komunikasi. Three-way handshake membantu membangun fondasi koneksi yang andal dan efisien dalam jaringan komputer.
