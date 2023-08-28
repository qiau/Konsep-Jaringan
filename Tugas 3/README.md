![Image Link]([https://github.com/qiau/Konsep-Jaringan/blob/main/Tugas%203/assets/tcp-udp-comparison-diagram-2.jpg](https://github.com/qiau/Konsep-Jaringan/blob/main/Tugas%203/assets/tcp-udp-comparison-diagram-2.jpg))

- # __PENGERTIAN__
#### _~ FTP (File Transfer Protocol)_
##### FTP adalah protokol yang digunakan untuk mentransfer file antara perangkat dalam jaringan. Ini memungkinkan pengguna untuk mengunggah (upload) dan mengunduh (download) file dari server ke klien dan sebaliknya. FTP dirancang dengan tujuan untuk mentransfer file dengan aman dan efisien. Protokol ini memiliki aturan dan komando tertentu yang mengatur cara berinteraksi dengan server FTP. FTP sendiri tidak mengatur secara khusus bagaimana data fisik dikirim, tetapi lebih berkaitan dengan perintah dan manajemen file.
#
#### _~ TCP (Transmission Control Protocol)_
##### TCP adalah protokol yang berfokus pada pengiriman data yang andal dan dijamin dalam jaringan. Protokol ini memastikan bahwa paket-paket data dikirimkan dengan benar, dalam urutan yang tepat, dan tanpa kehilangan. TCP menggunakan pendekatan yang lebih lambat dan lebih terkontrol untuk transfer data, karena protokol ini memerlukan konfirmasi pengiriman dan penanganan ulang paket-paket yang hilang atau rusak. Itu membuatnya cocok untuk aplikasi yang memerlukan keandalan, seperti transfer file atau laman web.
#
#### _~ UDP (User Datagram Protocol)_
##### UDP adalah protokol yang lebih sederhana dan lebih cepat dibandingkan dengan TCP. Ini dirancang untuk mentransfer data dengan sedikit overhead (beban tambahan) dan tanpa kebutuhan akan konfirmasi pengiriman atau penanganan ulang paket. Karena ini, UDP cocok untuk aplikasi yang membutuhkan kecepatan dan efisiensi lebih tinggi daripada keandalan mutlak. Contoh penggunaan UDP adalah streaming video dan game online.
#
#
#
- # Mengapa Dalam Satu Port FTP Terdapat Dua Protokol TCP dan UDP?
Pada dasarnya tidak ada satu port tunggal yang secara resmi ditetapkan untuk menggunakan baik TCP maupun UDP. Biasanya, protokol FTP lebih cenderung menggunakan TCP karena sifatnya yang memerlukan keandalan tinggi dan pengendalian. Namun, ada beberapa situasi di mana komunikasi dengan protokol FTP bisa melibatkan penggunaan UDP.
1. FTP Lebih Cocok dengan TCP:
FTP umumnya menggunakan TCP karena sifatnya yang memerlukan transfer file yang andal dan terkendali. TCP memastikan data dikirim dan diterima dengan benar serta dalam urutan yang tepat.

2. Mode Pasif FTP dengan TCP:
Dalam mode pasif FTP, komunikasi tetap menggunakan TCP untuk koneksi awal dan koneksi data baru yang diinisiasi oleh server.
3. Mode Aktif FTP Menggunakan TCP dan UDP:
Mode aktif FTP melibatkan koneksi awal melalui TCP dan kemudian koneksi data melalui port "aktif" yang bisa menggunakan UDP jika klien memilih mode aktif.
4. Jarang Penggunaan UDP dalam FTP:
Penggunaan UDP dalam FTP sangat jarang dan tidak umum. Ini bisa membingungkan dan rumit dalam manajemen keandalan dan pengendalian data.
5. Tergantung Konteks:
Jika menemukan port FTP dengan UDP, pastikan konteksnya. Kemungkinan besar ini adalah situasi khusus atau konfigurasi yang tidak umum.
6. Keandalan Prioritas Utama:
Dalam kebanyakan kasus, penggunaan TCP dengan FTP lebih diutamakan karena keandalan yang dibutuhkan untuk transfer file yang akurat.

Jadi, dalam kebanyakan kasus, protokol FTP menggunakan TCP karena sifatnya yang lebih cocok untuk keandalan dan pengendalian transfer file. Jika Anda menemukan situasi di mana port FTP menggunakan UDP, perlu diperhatikan bahwa ini mungkin dilakukan dalam konteks yang sangat khusus atau tidak standar.
