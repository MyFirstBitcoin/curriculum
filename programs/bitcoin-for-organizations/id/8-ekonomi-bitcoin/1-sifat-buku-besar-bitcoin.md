# 8.1 Sifat Buku Besar Bitcoin

Buku besar transaksi Bitcoin (juga dikenal sebagai timechain atau blockchain) adalah catatan publik yang dapat diakses, diberi cap waktu, dari setiap transaksi yang sah yang pernah terjadi di jaringan. Dalam sistem keuangan tradisional, transaksi internal hanya dapat dilihat oleh peserta yang berwenang, seperti bank, regulator, atau operator data seperti SWIFT, BACS, atau SEPA. Akses ke data pembayaran pada sistem tradisional bisa sangat terbatas dan mahal.

Sebaliknya, di dalam jaringan Bitcoin, siapa pun yang memiliki koneksi internet dapat melihat setiap transaksi mulai dari nilai terbesar hingga satuan Satoshi. Peserta dapat melacak total pasokan bitcoin secara real-time, memantau aktivitas alamat dan dompet, serta melihat imbalan penambang dan perilaku biaya transaksi. Meskipun aktivitas yang dapat dilihat di buku besar terhubung ke alamat kunci publik dan bukan identitas individu, tetap dimungkinkan untuk mengumpulkan kumpulan data besar tentang perilaku pengeluaran, sehingga semua orang dapat mengumpulkan dan meneliti aktivitas ekonomi secara real-time. Seiring pertumbuhan jaringan dan semakin diterima sebagai sumber kebenaran ekonomi, kita mungkin akan melihat ketergantungan yang lebih sedikit pada badan pemerintah dan penyedia pihak ketiga untuk produksi analisis statistik dan laporan perilaku pengeluaran.



#### 8.1.1 Node dan Block Explorer

Siapa pun yang ingin memverifikasi buku besar Bitcoin secara independen dan mengakses datanya sebaiknya menjalankan full node. Full node sering digambarkan sebagai cara paling mendasar untuk berpartisipasi dan memverifikasi ekonomi Bitcoin. Node ini tersedia secara global sebagai perangkat lunak open-source yang, ketika dijalankan, akan mengunduh dan memvalidasi seluruh buku besar Bitcoin mulai dari 'Genesis Block', yang diterbitkan pada Januari 2009, hingga hari ini. Node ini juga mendukung keamanan jaringan Bitcoin dengan membantu memverifikasi transaksi baru yang ditambahkan ke buku besar. Dengan mengakses buku besar Bitcoin dengan cara ini, full node berfungsi sebagai sumber kebenaran bagi peneliti dan auditor jaringan. Dan, bagi pengguna Bitcoin, full node bertindak sebagai gerbang 'kedaulatan diri' ke informasi transaksi ekonomi Bitcoin karena meningkatkan privasi dan keamanan dengan menghilangkan ketergantungan pada layanan pihak ketiga.

Sementara full node mengunduh data mentah, block explorer seperti mempool.space atau blockstream.info menawarkan antarmuka visual untuk mencari dan menafsirkan aktivitas buku besar. Block explorer memungkinkan transaksi individu untuk dilacak serta saldo dan riwayat dompet untuk dilihat. Ia juga menampilkan metrik aktivitas penambang seperti imbalan blok dan data biaya transaksi.

Bersama-sama, full node dan block explorer adalah alat yang membuat transparansi jaringan Bitcoin dapat digunakan.



#### 8.1.2 Aktivitas: Menjelajahi Buku Besar Bitcoin

1. Buka [mempool.space](https://mempool.space) dan jelajahi halaman utamanya.
  * Berapa tinggi blok terbaru?
  * Berapa biaya transaksi saat ini (Prioritas Rendah, Sedang, dan Tinggi)?
  * Berapa banyak transaksi yang menunggu di mempool untuk blok berikutnya
1. Akses blok terbaru di buku besar.
  * Berapa banyak transaksi yang disertakan?
  * Sebutkan penambang blok tersebut?
  * Berapa imbalan bloknya?
1. Akses salah satu transaksi dalam blok.
  * Berapa banyak input dan output yang dimiliki transaksi tersebut?
  * Berapa nilai transaksi dalam BTC dan USD?

Diskusikan perbedaan antara bagaimana uang bergerak dalam sistem lama dan bagaimana bisnis atau pemerintah menggunakan transparansi seperti ini.
