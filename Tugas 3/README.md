 Mengapa Dalam Satu Port FTP Terdapat Dua Protokol TCP dan UDP?
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
